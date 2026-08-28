<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hologram Data Display</title>
    <style>
        :root {
            --holo-cyan: #00f3ff;
            --holo-blue: #0066ff;
            --bg-dark: #030a16;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--bg-dark);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            overflow: hidden;
            color: #fff;
        }

        /* Hologram Container Wrapper */
        .holo-wrapper {
            position: relative;
            perspective: 1000px;
        }

        /* Base Grid Light under hologram */
        .holo-base {
            position: absolute;
            bottom: -30px;
            left: 50%;
            transform: translateX(-50%) rotateX(75deg);
            width: 300px;
            height: 300px;
            background: radial-gradient(circle, rgba(0, 243, 255, 0.4) 0%, transparent 70%);
            border-radius: 50%;
            box-shadow: 0 0 30px var(--holo-cyan);
            animation: basePulse 3s infinite alternate;
        }

        /* Main Hologram Card */
        .holo-card {
            position: relative;
            width: 380px;
            padding: 30px;
            background: rgba(0, 30, 60, 0.25);
            border: 1px solid rgba(0, 243, 255, 0.3);
            border-radius: 12px;
            backdrop-filter: blur(8px);
            box-shadow: 0 0 20px rgba(0, 243, 255, 0.15),
                        inset 0 0 15px rgba(0, 243, 255, 0.1);
            overflow: hidden;
            transform-style: preserve-3d;
            animation: float 4s ease-in-out infinite alternate;
        }

        /* Scanline Overlay Effect */
        .holo-card::before {
            content: '';
            position: absolute;
            top: 0; left: 0; right: 0; bottom: 0;
            background: linear-gradient(
                rgba(18, 16, 16, 0) 50%, 
                rgba(0, 243, 255, 0.15) 50%
            );
            background-size: 100% 4px;
            z-index: 2;
            pointer-events: none;
            opacity: 0.6;
        }

        /* Light Scanning Beam Effect */
        .holo-card::after {
            content: '';
            position: absolute;
            top: -100%;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(
                to bottom,
                transparent,
                rgba(0, 243, 255, 0.3),
                transparent
            );
            animation: scanBeam 4s cubic-bezier(0.4, 0, 0.2, 1) infinite;
            z-index: 3;
            pointer-events: none;
        }

        /* Header Style */
        .holo-header {
            border-bottom: 2px solid var(--holo-cyan);
            padding-bottom: 10px;
            margin-bottom: 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .holo-title {
            font-size: 1.2rem;
            letter-spacing: 2px;
            color: var(--holo-cyan);
            text-shadow: 0 0 8px var(--holo-cyan);
            text-transform: uppercase;
        }

        .status-dot {
            width: 8px;
            height: 8px;
            background-color: var(--holo-cyan);
            border-radius: 50%;
            box-shadow: 0 0 8px var(--holo-cyan);
            animation: blink 1s infinite alternate;
        }

        /* Item Stagger Animation (ค่อยๆ แสดงข้อมูล) */
        .data-item {
            margin-bottom: 15px;
            opacity: 0;
            transform: translateY(20px);
            animation: revealData 0.8s forwards ease-out;
        }

        /* Delay แต่ละรายการให้ค่อยๆ ปรากฏทีละอัน */
        .data-item:nth-child(1) { animation-delay: 0.3s; }
        .data-item:nth-child(2) { animation-delay: 0.6s; }
        .data-item:nth-child(3) { animation-delay: 0.9s; }
        .data-item:nth-child(4) { animation-delay: 1.2s; }

        .data-label {
            font-size: 0.8rem;
            color: #8ab4f8;
            text-transform: uppercase;
            letter-spacing: 1px;
            margin-bottom: 4px;
        }

        .data-value {
            font-size: 1.1rem;
            color: #fff;
            text-shadow: 0 0 5px var(--holo-cyan);
            font-weight: 600;
        }

        /* Keyframes Animations */
        @keyframes revealData {
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes scanBeam {
            0% { top: -100%; }
            100% { top: 200%; }
        }

        @keyframes float {
            0% { transform: translateY(0) rotateX(2deg); }
            100% { transform: translateY(-12px) rotateX(-2deg); }
        }

        @keyframes basePulse {
            0% { opacity: 0.3; transform: translateX(-50%) rotateX(75deg) scale(0.9); }
            100% { opacity: 0.7; transform: translateX(-50%) rotateX(75deg) scale(1.1); }
        }

        @keyframes blink {
            from { opacity: 0.3; }
            to { opacity: 1; }
        }
    </style>
</head>
<body>

    <div class="holo-wrapper">
        <div class="holo-base"></div>
        <div class="holo-card">
            <div class="holo-header">
                <span class="holo-title">SYSTEM STATUS</span>
                <div class="status-dot"></div>
            </div>

            <div class="data-container">
                <div class="data-item">
                    <div class="data-label">Core Target</div>
                    <div class="data-value">AI INTERFACE V.2026</div>
                </div>

                <div class="data-item">
                    <div class="data-label">Security Protocol</div>
                    <div class="data-value">ENCRYPTED // HIGH</div>
                </div>

                <div class="data-item">
                    <div class="data-label">Network Sync</div>
                    <div class="data-value">99.8% OPTIMAL</div>
                </div>

                <div class="data-item">
                    <div class="data-label">Location</div>
                    <div class="data-value">CHIANG MAI, THAILAND</div>
                </div>
            </div>
        </div>
    </div>

</body>
