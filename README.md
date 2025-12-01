<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Argly - App Support</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary: #6366f1;
            --secondary: #8b5cf6;
            --accent: #ec4899;
            --dark: #0f172a;
            --dark-secondary: #1e293b;
            --light: #f8fafc;
            --text: #e2e8f0;
            --text-muted: #94a3b8;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
            background: #0f172a;
            color: var(--text);
            line-height: 1.6;
            min-height: 100vh;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem;
        }

        header {
            text-align: center;
            padding: 4rem 0 2rem;
            position: relative;
        }

        .logo {
            font-size: 4rem;
            font-weight: 700;
            color: var(--primary);
            margin-bottom: 1rem;
            letter-spacing: -2px;
        }

        .tagline {
            font-size: 1.25rem;
            color: var(--text-muted);
            margin-bottom: 3rem;
        }

        .card {
            background: rgba(30, 41, 59, 0.8);
            border-radius: 20px;
            padding: 2.5rem;
            margin-bottom: 2rem;
            border: 1px solid rgba(99, 102, 241, 0.2);
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
        }

        .card h2 {
            color: var(--primary);
            font-size: 2rem;
            margin-bottom: 1.5rem;
            display: flex;
            align-items: center;
            gap: 0.75rem;
        }

        .card h3 {
            color: var(--secondary);
            font-size: 1.5rem;
            margin: 1.5rem 0 1rem;
        }

        .feature-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 1.5rem;
            margin: 2rem 0;
        }

        .feature-item {
            background: rgba(99, 102, 241, 0.1);
            padding: 1.5rem;
            border-radius: 12px;
            border-left: 4px solid var(--primary);
        }

        .feature-item strong {
            color: var(--secondary);
            display: block;
            margin-bottom: 0.5rem;
            font-size: 1.1rem;
        }

        ul {
            list-style: none;
            padding-left: 0;
        }

        ul li {
            padding: 0.75rem 0;
            padding-left: 1.5rem;
            position: relative;
        }

        ul li:before {
            content: "▸";
            position: absolute;
            left: 0;
            color: var(--primary);
            font-weight: bold;
        }

        .contact-section {
            text-align: center;
            padding: 3rem 0;
        }

        .contact-link {
            display: inline-block;
            padding: 1rem 2.5rem;
            background: var(--primary);
            color: white;
            text-decoration: none;
            border-radius: 50px;
            font-size: 1.1rem;
            font-weight: 600;
            box-shadow: 0 4px 12px rgba(99, 102, 241, 0.3);
        }

        .badge {
            display: inline-block;
            padding: 0.5rem 1rem;
            background: rgba(99, 102, 241, 0.2);
            border: 1px solid var(--primary);
            border-radius: 20px;
            font-size: 0.9rem;
            margin: 0.25rem;
        }

        .requirements {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
            margin: 2rem 0;
        }

        .requirement-box {
            background: rgba(139, 92, 246, 0.1);
            padding: 1.5rem;
            border-radius: 12px;
            border-top: 3px solid var(--secondary);
        }

        .requirement-box h4 {
            color: var(--secondary);
            margin-bottom: 0.75rem;
        }

        footer {
            text-align: center;
            padding: 3rem 0;
            color: var(--text-muted);
            border-top: 1px solid rgba(99, 102, 241, 0.2);
            margin-top: 4rem;
        }

        @media (max-width: 768px) {
            .logo {
                font-size: 2.5rem;
            }

            .card {
                padding: 1.5rem;
            }

            .feature-grid {
                grid-template-columns: 1fr;
            }
        }

        .icon {
            font-size: 1.5rem;
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <div class="logo">Argly</div>
            <div class="tagline">Remote Desktop Control</div>
        </header>

        <div class="card">
            <h2><span class="icon">✨</span> About Argly</h2>
            <p>
                Argly is a lightning-fast remote desktop application that allows you to control your macOS desktop 
                from your iOS device over your local network. Experience desktop-class performance with ultra-low 
                latency streaming—no internet connection required.
            </p>
            <p style="margin-top: 1rem; color: var(--text-muted);">
                Optimized for local network performance, Argly provides a seamless, 
                private, and secure way to access and control your Mac from anywhere in your home.
            </p>
        </div>

        <div class="card">
            <h2><span class="icon">🚀</span> Key Features</h2>
            <div class="feature-grid">
                <div class="feature-item">
                    <strong>🖥️ Real-Time Screen Sharing</strong>
                    Ultra-low latency screen mirroring with adaptive quality streaming and HD mode support.
                </div>
                <div class="feature-item">
                    <strong>🖱️ Full Desktop Control</strong>
                    Precise mouse, trackpad, and keyboard control with window dragging capabilities.
                </div>
                <div class="feature-item">
                    <strong>⌨️ Smart Keyboard</strong>
                    Custom keyboard overlay with quick shortcuts and haptic feedback.
                </div>
                <div class="feature-item">
                    <strong>🔓 Lock Screen Unlock</strong>
                    Unlock your Mac directly from your iPhone, even when it's locked.
                </div>
                <div class="feature-item">
                    <strong>🔍 Zero Configuration</strong>
                    Automatic device discovery—no setup required.
                </div>
                <div class="feature-item">
                    <strong>🔒 Privacy First</strong>
                    100% local network—all data stays on your network.
                </div>
            </div>
        </div>

        <div class="card">
            <h2><span class="icon">📋</span> Requirements</h2>
            <div class="requirements">
                <div class="requirement-box">
                    <h4>iOS Client</h4>
                    <p>iOS 15.0 or later</p>
                    <p style="color: var(--text-muted); margin-top: 0.5rem;">iPhone or iPad</p>
                </div>
                <div class="requirement-box">
                    <h4>macOS Server</h4>
                    <p>macOS 12.3 or later</p>
                    <p style="color: var(--text-muted); margin-top: 0.5rem;">Accessibility & Screen Recording permissions</p>
                </div>
                <div class="requirement-box">
                    <h4>Network</h4>
                    <p>Same Wi-Fi network</p>
                    <p style="color: var(--text-muted); margin-top: 0.5rem;">Local network connection required</p>
                </div>
            </div>
        </div>

        <div class="card">
            <h2><span class="icon">🛠️</span> Getting Started</h2>
            <h3>macOS Server Setup</h3>
            <ul>
                <li>Launch Argly Server on your Mac</li>
                <li>Click "Start Server"</li>
                <li>Grant accessibility and screen recording permissions when prompted</li>
                <li>Your Mac will automatically appear in the iOS app</li>
            </ul>

            <h3>iOS Client Setup</h3>
            <ul>
                <li>Open Argly on your iPhone or iPad</li>
                <li>Ensure both devices are on the same Wi-Fi network</li>
                <li>Your Mac will appear automatically in the device list</li>
                <li>Tap to connect and start controlling your Mac!</li>
            </ul>
        </div>

        <div class="card">
            <h2><span class="icon">💡</span> Use Cases</h2>
            <ul>
                <li><strong>Work from anywhere</strong> - Control your Mac from your couch or bed</li>
                <li><strong>Mobile presentations</strong> - Present from your iPhone</li>
                <li><strong>Remote unlock</strong> - Unlock your Mac when away from your desk</li>
                <li><strong>Quick file access</strong> - Access files and apps remotely</li>
                <li><strong>Media control</strong> - Control media playback from your phone</li>
            </ul>
        </div>

        <div class="card">
            <h2><span class="icon">🔐</span> Privacy & Security</h2>
            <p>
                Argly operates entirely on your local network. 
                All communication is direct between your devices. Optional password protection adds 
                an extra layer of security.
            </p>
            <div style="margin-top: 1.5rem;">
                <span class="badge">100% Local Network</span>
                <span class="badge">End-to-End Private</span>
                <span class="badge">Optional Password Protection</span>
            </div>
        </div>

        <div class="contact-section">
            <h2 style="color: var(--primary); margin-bottom: 1.5rem;">Need Help?</h2>
            <p style="color: var(--text-muted); margin-bottom: 2rem;">
                For support, questions, or feedback, please contact:
            </p>
            <a href="mailto:timnuwin@gmail.com" class="contact-link">timnuwin@gmail.com</a>
        </div>

        <footer>
            <p>Made with ❤️</p>
            <p style="margin-top: 0.5rem; color: var(--text-muted);">© 2025 Argly. All rights reserved.</p>
        </footer>
    </div>
</body>
</html>

