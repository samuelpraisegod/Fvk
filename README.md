<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>

🌐

 MarketFlow - Collaborative Trading Platform</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-
awesome/6.4.2/css/all.min.css" integrity="sha512-
z3gLpd7yknf1YoNbCzqRKc4qyor8gaKU1qmn+CShxbuBusANI9QpRohGBreCFk
KxLhei6S9CQXFEbbKuqLg0DA==" crossorigin="anonymous" 
referrerpolicy="no-referrer" />
    <style>
        :root {
            --primary: #0a1f44;
            --secondary: #d4af37;
            --light-bg: #f9f9f9;
            --white: #fff;
            --text: #333;
            --shadow: rgba(0, 0, 0, 0.1);
            --success: #28a745;
            --warning: #ffc107;
            --danger: #dc3545;
            --dark-red: #4a2626;
            --google-blue: #4285f4;
            --facebook-blue: #3b5998;
        }
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Segoe UI', sans-serif;
            background-color: var(--light-bg);
            color: var(--text);
            line-height: 1.6;
            scroll-behavior: smooth;
        }
        header {
            background: var(--dark-red);
            color: var(--white);
            padding: 1rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 2px 5px var(--shadow);
            position: sticky;
top: 0;
            z-index: 1000;
        }
        .logo {
            height: 50px;
        }
        .header-title {
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }
        header h1 {
            font-size: 1.8rem;
            color: var(--secondary);
        }
        nav ul {
            list-style: none;
            display: flex;
            gap: 1.5rem;
        }
        nav a {
            color: var(--white);
            text-decoration: none;
            font-weight: bold;
            transition: color 0.3s;
        }
        nav a:hover {
            color: var(--secondary);
        }
        .btn {
            padding: 0.75rem 1.5rem;
            border-radius: 5px;
            text-decoration: none;
            font-weight: bold;
            cursor: pointer;
            transition: background 0.3s;
            display: inline-block;
        }
        .btn-primary {
            background: var(--secondary);
            color: var(--primary);
        }
        .btn-primary:hover {
            background: #c49d2a;
        }
        .btn-success {
            background: var(--success);
}
        .btn-success:hover {
            background: #218838;
        }
        .btn-danger {
            background: var(--danger);
        }
        .btn-danger:hover {
            background: #c82333;
        }
        .btn-login {
            background: var(--white);
            color: var(--dark-red);
        }
        .btn-login:hover {
            background: #e0e0e0;
        }
        .btn-google {
            background: var(--google-blue);
            color: var(--white);
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }
        .btn-google:hover {
            background: #3267d6;
        }
        .btn-facebook {
            background: var(--facebook-blue);
            color: var(--white);
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }
        .btn-facebook:hover {
            background: #2f4b7c;
        }
        .hero {
            background: linear-gradient(to right, var(--dark-red), #6b3a3a);
            color: var(--white);
            text-align: center;
            padding: 4rem 2rem;
            margin-bottom: 2rem;
        }
        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
color: var(--secondary);
        }
        .hero p {
            font-size: 1.2rem;
            max-width: 600px;
            margin: 0 auto 1.5rem;
        }
        .hero .btn-container {
            display: flex;
            justify-content: center;
            gap: 1rem;
        }
        .section {
            padding: 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }
        .about, .features, .form-section, .traders-section {
            background: var(--white);
            border-radius: 8px;
            box-shadow: 0 4px 10px var(--shadow);
            margin-bottom: 2rem;
            padding: 2rem;
        }
        .about h2, .features h2, .form-section h2, .traders-section h2 {
            color: var(--primary);
            margin-bottom: 1rem;
        }
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
        }
        .feature-card {
            background: var(--light-bg);
            padding: 1.5rem;
            border-radius: 8px;
            text-align: center;
            transition: transform 0.3s;
        }
        .feature-card:hover {
            transform: translateY(-5px);
        }
        .feature-card h3 {
            color: var(--secondary);
            margin-bottom: 0.5rem;
        }
.form-section {
            background: var(--dark-red);
            color: var(--white);
        }
        .form-section h2, .form-section h3 {
            color: var(--secondary);
        }
        .form-group {
            margin-bottom: 1rem;
        }
        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
        }
        .form-group input, .form-group select, .form-group textarea {
            width: 100%;
            padding: 0.5rem;
            border: 1px solid var(--white);
            border-radius: 5px;
            background: var(--light-bg);
            color: var(--text);
        }
        .form-group input[type="file"] {
            width: auto;
        }
        .form-group textarea {
            height: 100px;
            resize: vertical;
        }
        .form-group button {
            background: var(--white);
            color: var(--dark-red);
            padding: 0.75rem 1.5rem;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .form-group button:hover {
            background: #e0e0e0;
        }
        .form-description {
            background: var(--light-bg);
            padding: 1rem;
            margin-bottom: 1rem;
            border-radius: 5px;
            font-style: italic;
        }
.social-login {
            display: flex;
            flex-direction: column;
            gap: 0.75rem;
            margin-bottom: 1.5rem;
        }
        .separator {
            text-align: center;
            margin: 1rem 0;
            font-weight: bold;
            color: var(--white);
        }
        .login-link a {
            color: var(--secondary);
            text-decoration: none;
        }
        .login-link a:hover {
            text-decoration: underline;
        }
        .fingerprint-icon {
            cursor: pointer;
            vertical-align: middle;
            margin-left: 0.5rem;
        }
        .dashboard {
            display: grid;
            grid-template-columns: 250px 1fr;
            min-height: calc(100vh - 60px);
        }
        .sidebar {
            background: var(--white);
            padding: 1.5rem;
            box-shadow: 2px 0 5px var(--shadow);
            position: sticky;
            top: 60px;
            height: calc(100vh - 60px);
            overflow-y: auto;
        }
        .sidebar ul {
            list-style: none;
            display: flex;
            flex-direction: column;
            gap: 0.5rem;
        }
        .sidebar a {
            color: var(--primary);
            text-decoration: none;
font-weight: bold;
            padding: 0.75rem;
            display: block;
            border-radius: 5px;
            transition: background 0.3s;
        }
        .sidebar a:hover {
            background: var(--light-bg);
            color: var(--secondary);
        }
        .main-content {
            padding: 2rem;
        }
        table {
            width: 100%;
            border-collapse: collapse;
        }
        th, td {
            padding: 0.75rem;
            text-align: left;
            border-bottom: 1px solid #ccc;
        }
        th {
            background: var(--light-bg);
        }
        .status {
            padding: 0.5rem;
            border-radius: 5px;
            color: var(--white);
            text-align: center;
        }
        .status-active {
            background: var(--success);
        }
        .status-pending {
            background: var(--warning);
        }
        .status-funded {
            background: var(--success);
        }
        .status-dispute {
            background: var(--danger);
        }
        .btn-secondary {
            background: var(--secondary);
            color: var(--primary);
        }
.btn-secondary:hover {
            background: #c49d2a;
        }
        .profile-info p {
            margin: 0.5rem 0;
        }
        .verification-section, .certificates-section {
            margin-top: 1rem;
            padding-top: 1rem;
            border-top: 1px solid #ccc;
        }
        .certificate-list li {
            background: var(--light-bg);
            padding: 0.5rem;
            margin-bottom: 0.5rem;
            border-radius: 5px;
            display: flex;
            justify-content: space-between;
        }
        .certificate-badge {
            background: var(--success);
            color: var(--white);
            padding: 0.25rem 0.5rem;
            border-radius: 5px;
            font-size: 0.8rem;
        }
        .chart-container {
            max-width: 600px;
            margin: 1rem auto;
        }
        .chat-box {
            border: 1px solid #ccc;
            border-radius: 5px;
            padding: 1rem;
            height: 300px;
            overflow-y: auto;
            background: #f5f5f5;
            margin-bottom: 1rem;
        }
        .chat-message {
            padding: 0.5rem;
            margin: 0.5rem;
            border-radius: 5px;
        }
        .chat-message.sent {
            background: var(--primary);
            color: var(--white);
margin-left: 20%;
        }
        .chat-message.received {
            background: #e0e0e0;
            margin-right: 20%;
        }
        .chat-input {
            display: flex;
            gap: 0.5rem;
        }
        .chat-input input {
            flex: 1;
            padding: 0.5rem;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.5);
            justify-content: center;
            align-items: center;
            z-index: 1000;
        }
        .modal-content {
            background: var(--dark-red);
            color: var(--white);
            padding: 1.5rem;
            border-radius: 8px;
            width: 90%;
            max-width: 600px;
            max-height: 80vh;
            overflow-y: auto;
        }
        .modal-content h2, .modal-content h3 {
            color: var(--secondary);
        }
        .close-btn {
            float: right;
            font-size: 1.5rem;
            cursor: pointer;
            color: var(--white);
        }
.close-btn:hover {
            color: var(--secondary);
        }
        .tabs {
            display: flex;
            gap: 1rem;
            margin-bottom: 1rem;
        }
        .tab-btn {
            padding: 0.5rem 1rem;
            border: none;
            background: var(--light-bg);
            cursor: pointer;
            border-radius: 5px;
            font-weight: bold;
        }
        .tab-btn.active {
            background: var(--primary);
            color: var(--white);
        }
        .tab-btn:hover {
            background: var(--secondary);
            color: var(--primary);
        }
        .tab-content {
            display: none;
        }
        .tab-content.active {
            display: block;
        }
        .hidden {
            display: none;
        }
        .view-toggle {
            margin-bottom: 1rem;
            display: flex;
            gap: 0.5rem;
        }
        .view-table {
            display: block;
        }
        .view-card {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1rem;
        }
        .view-card .feature-card {
background: var(--light-bg);
            padding: 1rem;
            border-radius: 8px;
        }
        .view-card .feature-card h3 {
            color: var(--primary);
        }
        footer {
            text-align: center;
            padding: 1rem;
        }
        footer a {
            color: var(--secondary);
            text-decoration: none;
        }
        footer a:hover {
            text-decoration: underline;
        }
        .social-icons {
            margin-top: 1rem;
            display: flex;
            justify-content: center;
            gap: 1rem;
        }
        .social-icons a {
            color: var(--secondary);
            font-size: 1.5rem;
            transition: color 0.3s;
        }
        .social-icons a:hover {
            color: var(--primary);
        }
        .error-message {
            color: var(--danger);
            font-size: 0.875rem;
            margin-top: 0.25rem;
        }
        .loading {
            opacity: 0.7;
            cursor: not-allowed;
        }
        .matching-section {
            margin-top: 1rem;
        }
        .matching-table {
            margin-top: 1rem;
        }
@media (max-width: 768px) {
            header {
                flex-direction: column;
                gap: 1rem;
            }
            nav ul {
                flex-direction: column;
                text-align: center;
            }
            .hero h1 {
                font-size: 1.8rem;
            }
            .hero p {
                font-size: 1rem;
            }
            .hero .btn-container {
                flex-direction: column;
                gap: 0.75rem;
            }
            .btn {
                width: 100%;
                max-width: 300px;
            }
            .dashboard {
                grid-template-columns: 1fr;
            }
            .sidebar {
                position: static;
                height: auto;
                box-shadow: none;
                border-bottom: 2px solid var(--shadow);
                padding: 1rem;
            }
            .sidebar ul {
                gap: 0.3rem;
            }
            .sidebar a {
                padding: 0.5rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <img src="assets/logo.png" alt="MarketFlow Logo" class="logo">
        <div class="header-title">
            <h1>MarketFlow</h1>
<span>

🌐

</span>
        </div>
        <nav>
            <ul id="nav-links">
                <li class="nav-home"><a href="#home">Home</a></li>
                <li class="nav-about"><a href="#about">About</a></li>
                <li class="nav-features"><a href="#features">Features</a></li>
                <li><a href="#" onclick="openTermsModal()">Terms & Conditions</
a></li>
                <li><a href="#" id="auth-btn" class="btn btn-primary">Login</a></
li>
            </ul>
        </nav>
    </header>
    <div id="home-content">
        <div class="hero">
            <h1>MarketFlow: The Trust-Driven Platform Where Traders Team Up</
h1>
            <p>Collaborate securely with traders to co-fund prop firm accounts, 
share profits, and trade with confidence.</p>
            <div class="btn-container">
                <a href="#signup" class="btn btn-primary">Get Started</a>
                <a href="#" class="btn btn-login" onclick="login()">Login</a>
            </div>
        </div>
        <div class="section about" id="about">
            <h2>About MarketFlow</h2>
            <p>MarketFlow empowers traders by providing tools, trust, and 
transparency. It enables:</p>
            <ul>
                <li>Co-funding prop firm accounts via a secure escrow system.</li>
                <li>From/to/mentions: Secure sharing of account access with 
encryption.</li>
                <li>Automated profit-sharing agreements.</li>
                <li>Performance tracking and fair partnerships.</li>
            </ul>
            <p>Our mission is to bridge the trust gap, reduce entry barriers, and 
ensure secure profit distribution.</p>
        </div>
        <div class="section features" id="features">
            <h2>Key Features</h2>
            <div class="features-grid">
                <div class="feature-card">
                    <h3>Trader Matchmaking</h3>
                    <p>Connect with traders for co-funding or collaboration.</p>
                </div>
                <div class="feature-card">
<h3>Escrow Funding</h3>
                    <p>Funds are held securely until terms are agreed.</p>
                </div>
                <div class="feature-card">
                    <h3>Profit-Sharing</h3>
                    <p>Define clear profit splits before trading.</p>
                </div>
                <div class="feature-card">
                    <h3>Secure Login</h3>
                    <p>Share credentials safely with encryption.</p>
                </div>
                <div class="feature-card">
                    <h3>Dashboard</h3>
                    <p>Monitor deals, profits, and settlements in real-time.</p>
                </div>
            </div>
        </div>
        <div class="section form-section" id="signup">
            <h2>Sign Up & Start Trading</h2>
            <div class="social-login">
                <button class="btn btn-google" onclick="signUpWithGoogle()">
                    <svg width="18" height="18" viewBox="0 0 24 24" fill="none" 
xmlns="http://www.w3.org/2000/svg">
                        <path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 
10-10S17.52 2 12 2zm0 18c-4.41 0-8-3.59-8-8s3.59-8 8-8 8 3.59 8 8-3.59 
8-8 
8zm4.83-12.55h-1.34v1.34h-1.34V7.45h-1.34v1.34H9.83V7.45H8.49v1.34H7.15
v1.34h1.34v1.34h1.34V10.13h1.34v1.34h1.34V10.13h1.34v1.34h1.34V8.79h-1.34
V7.45z" fill="white"/>
                    </svg>
                    Sign up with Google
                </button>
                <button class="btn btn-facebook" onclick="signUpWithFacebook()">
                    <svg width="18" height="18" viewBox="0 0 24 24" fill="none" 
xmlns="http://www.w3.org/2000/svg">
                        <path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 
10-10S17.52 2 12 2zm3.36 14.83h-2.07v-4.43h-1.97v-1.52h1.97V9.47c0-2.07 
1.24-3.20 
3.13-3.20h1.92v1.52h-1.39c-.91 0-1.08 .43-1.08 1.07v1.97h2.47l-.32 
1.52h-2.15v4.43z" fill="white"/>
                    </svg>
                    Sign up with Facebook
                </button>
            </div>
            <div class="separator">Or</div>
            <h3>Register with Email</h3>
            <form id="signup-form">
                <div class="form-group">
<label for="full-name">Full Name:</label>
                    <input type="text" id="full-name" name="full-name" 
placeholder="Enter your full name" required>
                </div>
                <div class="form-group">
                    <label for="email">Email:</label>
                    <input type="email" id="email" name="email" placeholder="Enter 
your email" required>
                </div>
                <div class="form-group">
                    <label for="role">Role:</label>
                    <select id="role" name="role" required>
                        <option value="">Select Role</option>
                        <option value="trader">Trader</option>
                        <option value="investor">Investor</option>
                    </select>
                </div>
                <div class="form-group">
                    <label for="amount">Amount to Fund (USD):</label>
                    <input type="number" id="amount" name="amount" min="0" 
placeholder="Enter amount" required>
                </div>
                <div class="form-group">
                    <label for="amount-description">Amount Description:</label>
                    <textarea id="amount-description" name="amount-description" 
placeholder="Describe your funding contribution or requirements"></textarea>
                </div>
                <div class="form-group">
                    <label for="profit-split">Profit Split (% Trader):</label>
                    <select id="profit-split" name="profit-split" required>
                        <option value="">Select Split</option>
                        <option value="50">50/50</option>
                        <option value="60">60/40</option>
                        <option value="70">70/30</option>
                    </select>
                </div>
                <div class="form-group">
                    <label>
                        <input type="checkbox" name="terms" required> I agree to the 
                        <a href="#" onclick="openTermsModal()">Terms & Conditions</
a>
                        <svg class="fingerprint-icon" onclick="openTermsModal()" 
width="18" height="18" viewBox="0 0 24 24" fill="none" xmlns="http://
www.w3.org/2000/svg">
                            <path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 
10-10S17.52 2 12 2zm0 18c-4.41 0-8-3.59-8-8s3.59-8 8-8 8 3.59 8 8-3.59 
8-8 8zm-1-14c-1.66 0-3 1.34-3 3 0 .55.15 1.06.41 1.5.55 1.01 1.47 1.73 2.59
1.73s2.04-.72 2.59-1.73c.26-.44.41-.95.41-1.5 0-1.66-1.34-3-3-3zm0 2c.55 0 
1 .45 1 1s-.45 1-1 1-1-.45-1-1 .45-1 1-1zm0 4c-2.76 0-5 2.24-5 
5v1h10v-1c0-2.76-2.24-5-5-5zm0 2c1.66 0 3 1.34 3 3H7c0-1.66 1.34-3 3-3z" 
fill="var(--secondary)"/>
                        </svg>
                    </label>
                </div>
                <div class="form-group">
                    <button type="submit" class="btn btn-primary">Submit</button>
                </div>
            </form>
            <div class="login-link">
                <p>Already have an account? <a href="#" onclick="login()">Login</
a></p>
            </div>
        </div>
    </div>
    <div id="dashboard-content" class="hidden">
        <div class="dashboard">
            <nav class="sidebar">
                <ul>
                    <li><a href="#deposit">Deposit</a></li>
                    <li><a href="#co-funding-requests">Co-Funding Requests</a></
li>
                    <li><a href="#requests">Requests</a></li>
                    <li><a href="#active-orders">Active Orders</a></li>
                    <li><a href="#completed-orders">Completed Orders</a></li>
                    <li><a href="#available-funded">Available Funded Accounts</a></
li>
                    <li><a href="#available-traders">Available Traders</a></li>
                    <li><a href="#profits">Profits & Withdrawals</a></li>
                    <li><a href="#disputes">Disputes</a></li>
                    <li><a href="#chart">Performance Chart</a></li>
                    <li><a href="#message-center">Message Center</a></li>
                    <li><a href="#balance">Balance</a></li>
                </ul>
            </nav>
            <main class="main-content">
                <section id="profile" class="section">
                    <h2>Your Profile</h2>
                    <div class="profile-info">
                        <p><strong>Name:</strong> Samuel Praisegod</p>
                        <p><strong>Email:</strong> samuelpraisegod90@gmail.com</
p>
                        <p><strong>Role:</strong> Trader</p>
                        <p><strong>Joined:</strong> August 2025</p>
                    </div>
<div class="verification-section">
                        <h3>Verification</h3>
                        <p><strong>Status:</strong> <span class="status status-
active">Verified</span></p>
                        <p><strong>Documents Submitted:</strong> Government ID, 
Trading History</p>
                        <p><strong>Last Updated:</strong> August 15, 2025</p>
                        <button class="btn btn-primary">Upload New Documents</
button>
                    </div>
                    <div class="certificates-section">
                        <h3>Trading Certificates</h3>
                        <p>Upload certificates to boost investor confidence.</p>
                        <ul class="certificate-list" id="certificate-list">
                            <li>Prop Firm A Certificate - Issued: Jan 2025 <span 
class="certificate-badge">Verified</span></li>
                        </ul>
                        <button class="btn btn-primary" 
onclick="uploadCertificate()">Upload Certificate</button>
                    </div>
                    <button class="btn btn-primary" style="margin-top: 1rem;">Edit 
Profile</button>
                    <button class="btn btn-danger" style="margin-top: 1rem;" 
onclick="logout()">Logout</button>
                </section>
                <section id="deposit" class="section">
                    <h2>Deposit Funds</h2>
                    <div class="form-description">
                        <p>Add funds to your MarketFlow account to participate in co-
funding or trading activities. Select a payment method and enter the amount to 
deposit.</p>
                    </div>
                    <form id="deposit-form">
                        <div class="form-group">
                            <label for="deposit-amount">Deposit Amount (USD):</label>
                            <input type="number" id="deposit-amount" name="deposit-
amount" min="10" placeholder="Enter amount (minimum $10)" required>
                        </div>
                        <div class="form-group">
                            <label for="payment-method">Payment Method:</label>
                            <select id="payment-method" name="payment-method" 
required>
                                <option value="">Select Payment Method</option>
                                <option value="bank-transfer">Bank Transfer</option>
                                <option value="credit-card">Credit/Debit Card</option>
                                <option value="paypal">PayPal</option>
                                <option value="crypto">Cryptocurrency</option>
</select>
                        </div>
                        <div class="form-group">
                            <label for="deposit-note">Note (Optional):</label>
                            <textarea id="deposit-note" name="deposit-note" 
placeholder="Add any additional details about your deposit"></textarea>
                        </div>
                        <div class="form-group">
                            <button type="submit" class="btn btn-primary">Submit 
Deposit</button>
                        </div>
                    </form>
                    <h3>Deposit History</h3>
                    <table>
                        <thead>
                            <tr>
                                <th>Transaction ID</th>
                                <th>Amount (USD)</th>
                                <th>Payment Method</th>
                                <th>Date</th>
                                <th>Status</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr>
                                <td>#TXN002</td>
                                <td>500</td>
                                <td>Credit Card</td>
                                <td>August 20, 2025</td>
                                <td><span class="status status-active">Completed</
span></td>
                            </tr>
                        </tbody>
                    </table>
                </section>
                <section id="co-funding-requests" class="section">
                    <h2>Co-Funding Requests</h2>
                    <div class="form-description">
                        <p>Create a co-fund request by selecting an amount. Your 
deposit will be locked in escrow until matched. The system will match co-
funders and auto-purchase the prop firm account upon agreement.</p>
                    </div>
                    <form id="co-fund-request-form">
                        <div class="form-group">
                            <label for="co-fund-amount">Co-Fund Amount (e.g., $5k)</
label>
                            <select id="co-fund-amount" name="co-fund-amount"
required>
                                <option value="">Select Amount</option>
                                <option value="5k">$5,000</option>
                                <option value="10k">$10,000</option>
                                <option value="25k">$25,000</option>
                            </select>
                        </div>
                        <div class="form-group">
                            <label for="co-fund-ratio">Profit Ratio</label>
                            <select id="co-fund-ratio" name="co-fund-ratio" required>
                                <option value="">Select Ratio</option>
                                <option value="50">50/50</option>
                                <option value="60">60/40</option>
                                <option value="70">70/30</option>
                            </select>
                        </div>
                        <div class="form-group">
                            <label for="co-fund-deposit">Your Contribution ($)</label>
                            <input type="number" id="co-fund-deposit" name="co-fund-
deposit" placeholder="e.g., 2500" required>
                        </div>
                        <button type="submit" class="btn btn-primary">Create Co-Fund 
Request</button>
                    </form>
                    <div>
                        <h3>Your Co-Funding Requests (Requester View)</h3>
                        <div class="view-card">
                            <div class="feature-card">
                                <h5>Co-Fund Request #2341</h5>
                                <p><strong>My Locked Amount:</strong> $500</p>
                                <p><strong>Status:</strong> <span class="status status-
pending">Pending Match</span></p>
                            </div>
                            <div class="feature-card">
                                <h5>Co-Fund Request #2342</h5>
                                <p><strong>My Locked Amount:</strong> $500</p>
                                <p><strong>Status:</strong> <span class="status status-
funded">Fully Funded – System Will Purchase Prop Account Automatically</
span></p>
                            </div>
                        </div>
                    </div>
                    <div class="matching-section">
                        <h3>Matched Co-Funders (Accepter View)</h3>
                        <div class="view-toggle">
                            <button class="btn btn-secondary" 
onclick="toggleView('table', 'matching')">Table View</button>
<button class="btn btn-secondary" 
onclick="toggleView('card', 'matching')">Card View</button>
                        </div>
                        <div id="matching-table" class="view-table">
                            <table class="matching-table">
                                <thead>
                                    <tr>
                                        <th>Match ID</th>
                                        <th>Amount</th>
                                        <th>Ratio</th>
                                        <th>Co-Funder</th>
                                        <th>Status</th>
                                        <th>Actions</th>
                                    </tr>
                                </thead>
                                <tbody>
                                    <tr>
                                        <td>#MATCH001</td>
                                        <td>$5,000</td>
                                        <td>50/50</td>
                                        <td>John CoFunder</td>
                                        <td><span class="status status-pending">Pending 
Agreement</span></td>
                                        <td>
                                            <button class="btn btn-success" 
onclick="acceptMatch('#MATCH001')">Agree & Fund</button>
                                        </td>
                                    </tr>
                                </tbody>
                            </table>
                        </div>
                        <div id="matching-cards" class="view-card hidden">
                            <div class="feature-card">
                                <h5>Co-Fund Request #2341</h5>
                                <p><strong>Requester Locked Amount:</strong> $500</p>
                                <p><strong>Your Required Amount:</strong> $500</p>
                                <p><strong>Status:</strong> <span class="status status-
pending">Awaiting Your Deposit</span></p>
                                <button class="btn btn-success" 
onclick="acceptMatch('#MATCH001')">Deposit & Accept</button>
                            </div>
                            <div class="feature-card">
                                <h5>Co-Fund Request #2342</h5>
                                <p><strong>Requester Locked Amount:</strong> $500</p>
                                <p><strong>Your Required Amount:</strong> $500</p>
                                <p><strong>Status:</strong> <span class="status status-
funded">Fully Funded - System Will Purchase Prop Account Automatically</span></p>
                            </div>
                        </div>
                    </div>
                </section>
                <section id="requests" class="section">
                    <h2>Request System</h2>
                    <div class="tabs">
                        <button class="tab-btn active" onclick="openRequestTab('co-
funding')">Co-Funding</button>
                        <button class="tab-btn" onclick="openRequestTab('managed-
trading')">Managed Trading</button>
                        <button class="tab-btn" 
onclick="openRequestTab('teaming')">Teaming</button>
                        <button class="tab-btn" 
onclick="openRequestTab('dashboard')">Dashboard</button>
                        <button class="tab-btn" onclick="openRequestTab('managed-
account-request')">Managed Account Request</button>
                    </div>
                    <div id="co-funding" class="tab-content active">
                        <h3>Co-Funding Request</h3>
                        <div class="form-description">
                            <p>Use this form to request co-funding for a prop firm 
account. You'll share the account cost and profits with another trader based on 
your agreed contribution ratio. Provide your prop firm details, deposit amount, 
and trading history to find a co-funder.</p>
                        </div>
                        <form id="coFundingForm">
                            <div class="form-group">
                                <label for="prop-firm">Prop Firm Name</label>
                                <select id="prop-firm" name="prop-firm" required>
                                    <option value="">Select Prop Firm</option>
                                    <option value="ftmo">FTMO</option>
                                    <option value="myforexfunds">MyForexFunds</option>
                                    <option value="the5ers">The5ers</option>
                                </select>
                            </div>
                            <div class="form-group">
                                <label for="account-size">Account Size</label>
                                <select id="account-size" name="account-size" required>
                                    <option value="">Select Account Size</option>
                                    <option value="5k">$5,000</option>
                                    <option value="10k">$10,000</option>
                                    <option value="25k">$25,000</option>
                                </select>
                            </div>
                            <div class="form-group">
<label for="deposit-amount">Your Deposit Amount ($)</
label>
                                <input type="number" id="deposit-amount" 
name="deposit-amount" placeholder="e.g., 50" required>
                            </div>
                            <div class="form-group">
                                <label for="profit-split">Profit Split (%)</label>
                                <select id="profit-split" name="profit-split" required>
                                    <option value="">Select Split</option>
                                    <option value="50">50/50</option>
                                    <option value="60">60/40</option>
                                    <option value="70">70/30</option>
                                </select>
                            </div>
                            <div class="form-group">
                                <label for="strategy">Trading Strategy</label>
                                <select id="strategy" name="strategy" required>
                                    <option value="">Select Strategy</option>
                                    <option value="scalping">Scalping</option>
                                    <option value="swing">Swing</option>
                                    <option value="algo">Algo</option>
                                </select>
                            </div>
                            <div class="form-group">
                                <label for="track-record">Track Record (MT4/MT5, 
MyFXBook, FXBlue link)</label>
                                <input type="url" id="track-record" name="track-record" 
placeholder="Paste link here" required>
                            </div>
                            <div class="form-group">
                                <label for="certificate-file">Upload Certificate (Optional)</
label>
                                <input type="file" id="certificate-file" name="certificate-
file" accept=".pdf,.jpg,.png">
                            </div>
                            <button type="submit" class="btn btn-primary">Submit 
Request</button>
                        </form>
                    </div>
                    <div id="managed-trading" class="tab-content">
                        <h3>Managed Trading Account</h3>
                        <div class="form-description">
                            <p>This form is for traders who want to manage an investor's 
capital. Agree on the investment, type of account, profit targets, and return 
cycle. Investors control withdrawals, and profits are shared based on the 
agreed terms.</p>
                        </div>
<form id="managedTradingForm">
                            <div class="form-group">
                                <label for="investment-plan">Investment Plan (Capital 
Size)</label>
                                <input type="number" id="investment-plan" 
name="investment-plan" placeholder="e.g., 10000" required>
                            </div>
                            <div class="form-group">
                                <label for="account-type">Kind of Account</label>
                                <select id="account-type" name="account-type" required>
                                    <option value="">Select Account Type</option>
                                    <option value="forex">Forex</option>
                                    <option value="stocks">Stocks</option>
                                    <option value="crypto">Cryptocurrency</option>
                                    <option value="commodities">Commodities</option>
                                </select>
                            </div>
                            <div class="form-group">
                                <label for="return-cycle">Return Cycle</label>
                                <select id="return-cycle" name="return-cycle" required>
                                    <option value="">Select Cycle</option>
                                    <option value="daily">Daily</option>
                                    <option value="weekly">Weekly</option>
                                    <option value="monthly">Monthly</option>
                                    <option value="long-term">Long-term</option>
                                </select>
                            </div>
                            <div class="form-group">
                                <label for="profit-target">Profit Target (%)</label>
                                <input type="number" id="profit-target" name="profit-
target" placeholder="e.g., 10" required>
                            </div>
                            <div class="form-group">
                                <label for="withdrawal-terms">Withdrawal Terms</label>
                                <textarea id="withdrawal-terms" name="withdrawal-terms" 
placeholder="Describe profit split and withdrawal terms" required></textarea>
                            </div>
                            <button type="submit" class="btn btn-primary">Apply to 
Investor</button>
                        </form>
                    </div>
                    <div id="teaming" class="tab-content">
                        <h3>Teaming with Traders</h3>
                        <div class="form-description">
                            <p>Use this form to team up with another trader to pass a 
prop firm challenge. Provide details about the prop firm account, rules, and 
your contribution (slip amount). Both traders agree on terms, and progress is
tracked in the dashboard.</p>
                        </div>
                        <form id="teamingForm">
                            <div class="form-group">
                                <label for="team-prop-firm">Prop Firm Name</label>
                                <select id="team-prop-firm" name="team-prop-firm" 
required>
                                    <option value="">Select Prop Firm</option>
                                    <option value="ftmo">FTMO</option>
                                    <option value="myforexfunds">MyForexFunds</option>
                                    <option value="the5ers">The5ers</option>
                                </select>
                            </div>
                            <div class="form-group">
                                <label for="team-account-size">Account Size</label>
                                <select id="team-account-size" name="team-account-size" 
required>
                                    <option value="">Select Account Size</option>
                                    <option value="5k">$5,000</option>
                                    <option value="10k">$10,000</option>
                                    <option value="25k">$25,000</option>
                                </select>
                            </div>
                            <div class="form-group">
                                <label for="account-rules">Account Rules</label>
                                <textarea id="account-rules" name="account-rules" 
placeholder="Paste or describe account rules" required></textarea>
                            </div>
                            <div class="form-group">
                                <label for="slip-amount">Slip Amount ($)</label>
                                <input type="number" id="slip-amount" name="slip-
amount" placeholder="e.g., 50" required>
                            </div>
                            <button type="submit" class="btn btn-primary">Submit 
Teaming Request</button>
                        </form>
                    </div>
                    <div id="dashboard" class="tab-content">
                        <h3>Dashboard</h3>
                        <div class="form-description">
                            <p>View and manage all your requests and agreements here. 
Accept or decline pending requests, track active agreements, and monitor 
profit-sharing status.</p>
                        </div>
                        <div class="view-toggle">
                            <button class="btn btn-secondary" 
onclick="toggleView('table', 'dashboard')">Table View</button>
<button class="btn btn-secondary" 
onclick="toggleView('card', 'dashboard')">Card View</button>
                        </div>
                        <div id="dashboard-table" class="view-table">
                            <h4>Pending Requests</h4>
                            <table>
                                <thead>
                                    <tr>
                                        <th>Type</th>
                                        <th>Details</th>
                                        <th>Status</th>
                                        <th>Actions</th>
                                    </tr>
                                </thead>
                                <tbody>
                                    <tr>
                                        <td>Co-Funding</td>
                                        <td>FTMO, $10k, 50/50 split</td>
                                        <td><span class="status status-pending">Pending</
span></td>
                                        <td>
                                            <button class="btn btn-success" 
onclick="acceptRequest('Co-Funding')">Accept</button>
                                            <button class="btn btn-danger" 
onclick="declineRequest('Co-Funding')">Decline</button>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td>Managed Trading</td>
                                        <td>$5k, Weekly Returns</td>
                                        <td><span class="status status-pending">Pending</
span></td>
                                        <td>
                                            <button class="btn btn-success" 
onclick="acceptRequest('Managed Trading')">Accept</button>
                                            <button class="btn btn-danger" 
onclick="declineRequest('Managed Trading')">Decline</button>
                                        </td>
                                    </tr>
                                </tbody>
                            </table>
                            <h4>Active Agreements</h4>
                            <table>
                                <thead>
                                    <tr>
                                        <th>Type</th>
                                        <th>Details</th>
<th>Profit Status</th>
                                        <th>Actions</th>
                                    </tr>
                                </thead>
                                <tbody>
                                    <tr>
                                        <td>Co-Funding</td>
                                        <td>FTMO, $25k, 60/40 split</td>
                                        <td>Profit: $1,200 (Your share: $720)</td>
                                        <td>
                                            <button class="btn btn-primary" 
onclick="viewOrderDetails('Co-Funding')">View Details</button>
                                            <button class="btn btn-danger" 
onclick="fileDispute('Co-Funding')">File Dispute</button>
                                        </td>
                                    </tr>
                                </tbody>
                            </table>
                        </div>
                        <div id="dashboard-cards" class="view-card hidden">
                            <div class="feature-card">
                                <h3>Co-Funding Request</h3>
                                <p><strong>Details:</strong> FTMO, $10k, 50/50 split</p>
                                <p><strong>Status:</strong> <span class="status status-
pending">Pending</span></p>
                                <button class="btn btn-success" 
onclick="acceptRequest('Co-Funding')">Accept</button>
                                <button class="btn btn-danger" 
onclick="declineRequest('Co-Funding')">Decline</button>
                            </div>
                            <div class="feature-card">
                                <h3>Managed Trading Request</h3>
                                <p><strong>Details:</strong> $5k, Weekly Returns</p>
                                <p><strong>Status:</strong> <span class="status status-
pending">Pending</span></p>
                                <button class="btn btn-success" 
onclick="acceptRequest('Managed Trading')">Accept</button>
                                <button class="btn btn-danger" 
onclick="declineRequest('Managed Trading')">Decline</button>
                            </div>
                            <div class="feature-card">
                                <h3>Active Agreement</h3>
                                <p><strong>Details:</strong> FTMO, $25k, 60/40 split</p>
                                <p><strong>Profit Status:</strong> $1,200 (Your share: 
$720)</p>
                                <button class="btn btn-primary" 
onclick="viewOrderDetails('Co-Funding')">View Details</button>
<button class="btn btn-danger" onclick="fileDispute('Co-
Funding')">File Dispute</button>
                            </div>
                        </div>
                    </div>
                    <div id="managed-account-request" class="tab-content">
                        <h3>Managed Account Request</h3>
                        <div class="form-description">
                            <p>For investors: Create a managed account request to link 
with a trader without revealing sensitive broker details. Input your broker name, 
account ID, and the trader's platform ID. The system will securely connect 
you.</p>
                        </div>
                        <form id="managed-account-request-form">
                            <div class="form-group">
                                <label for="broker-name">Broker Name</label>
                                <input type="text" id="broker-name" name="broker-name" 
placeholder="e.g., BrokerXYZ" required>
                            </div>
                            <div class="form-group">
                                <label for="account-id">Account ID</label>
                                <input type="text" id="account-id" name="account-id" 
placeholder="e.g., ACC123456" required>
                            </div>
                            <div class="form-group">
                                <label for="trader-id">Trader's Platform ID</label>
                                <input type="text" id="trader-id" name="trader-id" 
placeholder="e.g., TRADER789" required>
                            </div>
                            <div class="form-group">
                                <label for="managed-profit-split">Profit Split (%)</label>
                                <select id="managed-profit-split" name="managed-profit-
split" required>
                                    <option value="">Select Split</option>
                                    <option value="50">50/50</option>
                                    <option value="60">60/40</option>
                                    <option value="70">70/30</option>
                                </select>
                            </div>
                            <button type="submit" class="btn btn-primary">Submit 
Managed Account Request</button>
                        </form>
                    </div>
                </section>
                <section id="active-orders" class="section">
                    <h2>Active Orders</h2>
                    <div class="view-toggle">
<button class="btn btn-secondary" onclick="toggleView('table', 
'active-orders')">Table View</button>
                        <button class="btn btn-secondary" onclick="toggleView('card', 
'active-orders')">Card View</button>
                    </div>
                    <div id="active-orders-table" class="view-table">
                        <table>
                            <thead>
                                <tr>
                                    <th>Order ID</th>
                                    <th>Type</th>
                                    <th>Trader/Investor</th>
                                    <th>Profit Split</th>
                                    <th>Funding Size</th>
                                    <th>Prop Firm</th>
                                    <th>Profit Share</th>
                                    <th>Status</th>
                                    <th>Actions</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>#ORD001</td>
                                    <td>Co-Funding</td>
                                    <td>Chidinma Obi</td>
                                    <td>50/50</td>
                                    <td>$5,000</td>
                                    <td>Partner Choice</td>
                                    <td>$500 (Your Share: $250)</td>
                                    <td><span class="status status-active">Active</span></
td>
                                    <td>
                                        <button class="btn btn-primary" 
onclick="viewOrderDetails('#ORD001')">View Details</button>
                                        <button class="btn btn-secondary" 
onclick="openChat('Chidinma Obi')">Chat</button>
                                        <button class="btn btn-danger" 
onclick="fileDispute('#ORD001')">File Dispute</button>
                                    </td>
                                </tr>
                            </tbody>
                        </table>
                    </div>
                    <div id="active-orders-cards" class="view-card hidden">
                        <div class="feature-card">
                            <h3>Order #ORD001</h3>
                            <p><strong>Type:</strong> Co-Funding</p>
<p><strong>Trader/Investor:</strong> Chidinma Obi</p>
                            <p><strong>Profit Split:</strong> 50/50</p>
                            <p><strong>Funding Size:</strong> $5,000</p>
                            <p><strong>Prop Firm:</strong> Partner Choice</p>
                            <p><strong>Profit Share:</strong> $500 (Your Share: $250)</
p>
                            <p><strong>Status:</strong> <span class="status status-
active">Active</span></p>
                            <button class="btn btn-primary" 
onclick="viewOrderDetails('#ORD001')">View Details</button>
                            <button class="btn btn-secondary" 
onclick="openChat('Chidinma Obi')">Chat</button>
                            <button class="btn btn-danger" 
onclick="fileDispute('#ORD001')">File Dispute</button>
                        </div>
                    </div>
                </section>
                <section id="completed-orders" class="section">
                    <h2>Completed Orders</h2>
                    <div class="view-toggle">
                        <button class="btn btn-secondary" onclick="toggleView('table', 
'completed-orders')">Table View</button>
                        <button class="btn btn-secondary" onclick="toggleView('card', 
'completed-orders')">Card View</button>
                    </div>
                    <div id="completed-orders-table" class="view-table">
                        <table>
                            <thead>
                                <tr>
                                    <th>Order ID</th>
                                    <th>Type</th>
                                    <th>Trader/Investor</th>
                                    <th>Profit Split</th>
                                    <th>Funding Size</th>
                                    <th>Prop Firm</th>
                                    <th>Final Profit</th>
                                    <th>Status</th>
                                    <th>Actions</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>#ORD002</td>
                                    <td>Trading for Investor</td>
                                    <td>John Investor</td>
                                    <td>60/40</td>
                                    <td>$10,000</td>
<td>FTMO</td>
                                    <td>$1,200 (Your Share: $720)</td>
                                    <td><span class="status status-active">Completed</
span></td>
                                    <td>
                                        <button class="btn btn-primary" 
onclick="viewOrderDetails('#ORD002')">View Details</button>
                                        <button class="btn btn-primary" 
onclick="downloadAgreement('#ORD002')">Download Agreement</button>
                                    </td>
                                </tr>
                            </tbody>
                        </table>
                    </div>
                    <div id="completed-orders-cards" class="view-card hidden">
                        <div class="feature-card">
                            <h3>Order #ORD002</h3>
                            <p><strong>Type:</strong> Trading for Investor</p>
                            <p><strong>Trader/Investor:</strong> John Investor</p>
                            <p><strong>Profit Split:</strong> 60/40</p>
                            <p><strong>Funding Size:</strong> $10,000</p>
                            <p><strong>Prop Firm:</strong> FTMO</p>
                            <p><strong>Final Profit:</strong> $1,200 (Your Share: 
$720)</p>
                            <p><strong>Status:</strong> <span class="status status-
active">Completed</span></p>
                            <button class="btn btn-primary" 
onclick="viewOrderDetails('#ORD002')">View Details</button>
                            <button class="btn btn-primary" 
onclick="downloadAgreement('#ORD002')">Download Agreement</button>
                        </div>
                    </div>
                </section>
                <section id="available-funded" class="section">
                    <h2>Available Funded Accounts</h2>
                    <table>
                        <thead>
                            <tr>
                                <th>Account ID</th>
                                <th>Funded Amount (USD)</th>
                                <th>Profit Split</th>
                                <th>Prop Firm</th>
                                <th>Certificate Status</th>
                                <th>Status</th>
                                <th>Actions</th>
                            </tr>
                        </thead>
<tbody>
                            <tr>
                                <td>#ACC003</td>
                                <td>10,000</td>
                                <td>60/40</td>
                                <td>FTMO</td>
                                <td><span class="certificate-badge">Verified (2 
Certificates)</span></td>
                                <td><span class="status status-active">Available</span></
td>
                                <td>
                                    <button class="btn btn-secondary" 
onclick="openChat('Account #ACC003')">Chat</button>
                                    <button class="btn btn-primary" 
onclick="requestMatch('Account #ACC003')">Request Match</button>
                                </td>
                            </tr>
                        </tbody>
                    </table>
                </section>
                <section id="available-traders" class="section">
                    <h2>Available Traders</h2>
                    <table>
                        <thead>
                            <tr>
                                <th>Trader Name</th>
                                <th>Experience Level</th>
                                <th>Preferred Profit Split</th>
                                <th>Experience Proof</th>
                                <th>Status</th>
                                <th>Actions</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr>
                                <td>Adebayo Chukwu</td>
                                <td>Advanced (3+ years)</td>
                                <td>60/40</td>
                                <td><span class="certificate-badge">Verified (2 
Certificates)</span></td>
                                <td><span class="status status-active">Available</span></
td>
                                <td>
                                    <button class="btn btn-secondary" 
onclick="openChat('Adebayo Chukwu')">Chat</button>
                                    <button class="btn btn-primary" 
onclick="requestMatch('Adebayo Chukwu')">Request Match</button>
                                </td>
                            </tr>
                        </tbody>
                    </table>
                </section>
                <section id="profits" class="section">
                    <h2>Profits & Withdrawals</h2>
                    <table>
                        <thead>
                            <tr>
                                <th>Account ID</th>
                                <th>Total Profits (USD)</th>
                                <th>Your Share (USD)</th>
                                <th>Status</th>
                                <th>Actions</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr>
                                <td>#ACC001</td>
                                <td>1500</td>
                                <td>900</td>
                                <td><span class="status status-active">Ready</span></
td>
                                <td><button class="btn btn-success">Request 
Withdrawal</button></td>
                            </tr>
                        </tbody>
                    </table>
                </section>
                <section id="disputes" class="section">
                    <h2>Disputes & Resolution</h2>
                    <table>
                        <thead>
                            <tr>
                                <th>Dispute ID</th>
                                <th>Account ID</th>
                                <th>Issue</th>
                                <th>Status</th>
                                <th>Actions</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr>
                                <td>#DSP001</td>
                                <td>#ACC001</td>
                                <td>Profit split disagreement</td>
<td><span class="status status-dispute">Open</span></
td>
                                <td><button class="btn btn-danger">View/Respond</
button></td>
                            </tr>
                        </tbody>
                    </table>
                </section>
                <section id="chart" class="section">
                    <h2>Performance Chart</h2>
                    <div class="chart-container">
                        <canvas id="performanceChart"></canvas>
                    </div>
                </section>
                <section id="message-center" class="section">
                    <h2>Message Center</h2>
                    <div class="tabs">
                        <button class="tab-btn active" onclick="openTab('co-
funded')">Co-Funded Messages</button>
                        <button class="tab-btn" 
onclick="openTab('support')">Customer Support</button>
                        <button class="tab-btn" onclick="openTab('traders-
group')">Join Traders Chat Group</button>
                    </div>
                    <div id="co-funded" class="tab-content active">
                        <div class="chat-box" id="coFundedChatBox">
                            <div class="chat-message received">John Investor: How’s the 
account performing?</div>
                            <div class="chat-message sent">You: Up $900 this month, 
check the profits section!</div>
                        </div>
                        <div class="chat-input">
                            <input type="text" id="coFundedChatInput" 
placeholder="Type your message...">
                            <button class="btn btn-primary" 
onclick="sendCoFundedMessage()">Send</button>
                        </div>
                    </div>
                    <div id="support" class="tab-content">
                        <div class="chat-box" id="supportChatBox">
                            <div class="chat-message received">Support: How can we 
assist you today?</div>
                            <div class="chat-message sent">You: Need help with 
withdrawal process.</div>
                        </div>
                        <div class="chat-input">
                            <input type="text" id="supportChatInput" placeholder="Type
your message...">
                            <button class="btn btn-primary" 
onclick="sendSupportMessage()">Send</button>
                        </div>
                    </div>
                    <div id="traders-group" class="tab-content">
                        <p>Join our Traders Community to connect with other traders!</
p>
                        <a href="https://t.me/MarketFlowpropTraders" target="_blank" 
class="btn btn-primary">Join Telegram Group</a>
                    </div>
                </section>
                <section id="balance" class="section">
                    <h2>Account Balance</h2>
                    <div class="profile-info">
                        <p><strong>Current Balance:</strong> $2,500 USD</p>
                        <p><strong>Pending Withdrawals:</strong> $400 USD</p>
                        <p><strong>Total Withdrawn:</strong> $1,200 USD</p>
                    </div>
                    <table>
                        <thead>
                            <tr>
                                <th>Transaction ID</th>
                                <th>Amount (USD)</th>
                                <th>Date</th>
                                <th>Type</th>
                                <th>Status</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr>
                                <td>#TXN001</td>
                                <td>900</td>
                                <td>August 10, 2025</td>
                                <td>Withdrawal</td>
                                <td><span class="status status-active">Completed</
span></td>
                            </tr>
                        </tbody>
                    </table>
                </section>
            </main>
        </div>
        <div id="chatModal" class="modal">
            <div class="modal-content">
                <span class="close-btn" onclick="closeChat()">&times;</span>
                <h3 id="chatTraderName">Chat with Trader</h3>
<div class="chat-box" id="traderChatBox"></div>
                <div class="chat-input">
                    <input type="text" id="traderChatInput" placeholder="Type your 
message...">
                    <button class="btn btn-primary" 
onclick="sendTraderMessage()">Send</button>
                </div>
            </div>
        </div>
        <div id="termsModal" class="modal">
            <div class="modal-content">
                <span class="close-btn" onclick="closeTermsModal()">&times;</
span>
                <h2>Terms & Conditions – Trader Collaboration & Profit Sharing</h2>
                <p><strong>Effective Date:</strong> August 23, 2025</p>
                <p><strong>Platform Name:</strong> MarketFlow</p>
                <h3>1. Acceptance of Terms</h3>
                <p>By registering on the Platform, you agree to these Terms & 
Conditions, which govern all collaborations, escrow services, profit-sharing 
agreements, and dispute resolutions.</p>
                <h3>2. Purpose of the Platform</h3>
                <p>The Platform acts as a neutral middleman to:</p>
                <ul>
                    <li>Facilitate collaboration between traders.</li>
                    <li>Securely hold and distribute profits according to agreed 
terms.</li>
                    <li>Provide a framework for dispute resolution and trust 
management.</li>
                </ul>
                <h3>3. Profit Sharing Agreements</h3>
                <ol>
                    <li>Before funding an account, traders must mutually agree on split 
terms (e.g., 60/40).</li>
                    <li>The agreed terms will be digitally recorded and signed inside 
the Platform.</li>
                    <li>The Platform will enforce the split automatically upon profit 
withdrawal.</li>
                </ol>
                <h3>4. Escrow & Withdrawals</h3>
                <ol>
                    <li>All profits must pass through the Platform’s escrow wallet.</li>
                    <li>Withdrawals are processed according to the recorded 
agreement.</li>
                    <li>No trader can unilaterally withdraw or modify the profit-sharing 
ratio once active.</li>
                    <li>Bypassing escrow may result in suspension and forfeiture of 
funds.</li>
</ol>
                <h3>5. Responsibilities of Traders</h3>
                <p>Traders must:</p>
                <ul>
                    <li>Fund accounts honestly and as agreed.</li>
                    <li>Provide accurate information (ID, account details, 
contributions).</li>
                    <li>Respect the agreed split and the Platform’s enforcement.</li>
                </ul>
                <p>The Platform is not responsible for trading losses or market 
risks.</p>
                <h3>6. Dispute Resolution</h3>
                <ol>
                    <li>Traders may submit a request for arbitration through the 
Platform.</li>
                    <li>Arbitration decisions are final and binding.</li>
                </ol>
                <h3>7. Reputation & Blacklisting</h3>
                <p>Traders who violate agreements may be flagged, blacklisted, or 
lose reputation scores.</p>
                <h3>8. Legal Framework</h3>
                <p>This agreement is a binding digital contract, governed by the laws 
of Delaware, USA.</p>
            </div>
        </div>
    </div>
    <footer>
        <p>&copy; 2025 MarketFlow | Contact: support@marketflowprop.com | <a 
href="#" onclick="openTermsModal()">Terms & Conditions</a></p>
        <div class="social-icons">
            <a href="https://x.com/MarketFlowProp" target="_blank" aria-
label="Follow us on Twitter/X"><i class="fab fa-x-twitter"></i></a>
            <a href="https://facebook.com/MarketFlowProp" target="_blank" aria-
label="Follow us on Facebook"><i class="fab fa-facebook-f"></i></a>
            <a href="https://instagram.com/MarketFlowProp" target="_blank" aria-
label="Follow us on Instagram"><i class="fab fa-instagram"></i></a>
            <a href="https://tiktok.com/@MarketFlowProp" target="_blank" aria-
label="Follow us on TikTok"><i class="fab fa-tiktok"></i></a>
        </div>
    </footer>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <script>
        let isLoggedIn = false;
        let currentTrader = '';

        function updateUI() {
            const homeContent = document.getElementById('home-content');
const dashboardContent = document.getElementById('dashboard-
content');
            const authBtn = document.getElementById('auth-btn');

            if (isLoggedIn) {
                homeContent.classList.add('hidden');
                dashboardContent.classList.remove('hidden');
                authBtn.textContent = 'Logout';
                authBtn.onclick = logout;
            } else {
                homeContent.classList.remove('hidden');
                dashboardContent.classList.add('hidden');
                authBtn.textContent = 'Login';
                authBtn.onclick = login;
            }

            document.querySelectorAll('nav a').forEach(anchor => {
                anchor.addEventListener('click', function (e) {
                    if (this.getAttribute('href').startsWith('#')) {
                        e.preventDefault();
                        
document.querySelector(this.getAttribute('href')).scrollIntoView({ behavior: 
'smooth' });
                    }
                });
            });

            document.querySelectorAll('.sidebar a').forEach(anchor => {
                anchor.addEventListener('click', function (e) {
                    if (this.getAttribute('href').startsWith('#')) {
                        e.preventDefault();
                        
document.querySelector(this.getAttribute('href')).scrollIntoView({ behavior: 
'smooth' });
                    }
                });
            });
        }

        function login() {
            isLoggedIn = true;
            updateUI();
            document.querySelector('#dashboard-
content').scrollIntoView({ behavior: 'smooth' });
        }

        function logout() {
isLoggedIn = false;
            updateUI();
            document.querySelector('#home-content').scrollIntoView({ behavior: 
'smooth' });
        }

        function signUpWithGoogle() {
            alert('Redirecting to Google authentication...');
        }

        function signUpWithFacebook() {
            alert('Redirecting to Facebook authentication...');
        }

        function openTermsModal() {
            document.getElementById('termsModal').style.display = 'flex';
        }

        function closeTermsModal() {
            document.getElementById('termsModal').style.display = 'none';
        }

        function uploadCertificate() {
            const certName = prompt('Enter certificate name (e.g., Prop Firm B 
Certificate):');
            if (certName) {
                const list = document.getElementById('certificate-list');
                const li = document.createElement('li');
                li.innerHTML = `${certName} <span class="certificate-
badge">Verified</span>`;
                list.appendChild(li);
                alert('Certificate uploaded successfully!');
            }
        }

        function openRequestTab(tabName) {
            document.querySelectorAll('#requests .tab-content').forEach(tab => {
                tab.classList.remove('active');
            });
            document.querySelectorAll('#requests .tab-btn').forEach(btn => {
                btn.classList.remove('active');
            });
            document.getElementById(tabName).classList.add('active');
            document.querySelector(`button[onclick="openRequestTab('$
{tabName}')"]`).classList.add('active');
        }
function toggleView(viewType, section) {
            const tableView = document.querySelector(`#${section}-table`);
            const cardView = document.querySelector(`#${section}-cards`);
            if (viewType === 'table') {
                tableView.style.display = 'block';
                cardView.style.display = 'none';
            } else {
                tableView.style.display = 'none';
                cardView.style.display = 'grid';
            }
        }

        function openChat(traderName) {
            currentTrader = traderName;
            document.getElementById('chatTraderName').textContent = `Chat with 
${traderName}`;
            document.getElementById('traderChatBox').innerHTML = `<div 
class="chat-message received">${traderName}: Hi, interested in co-funding? 
Let's discuss!</div>`;
            document.getElementById('chatModal').style.display = 'flex';
        }

        function closeChat() {
            document.getElementById('chatModal').style.display = 'none';
            document.getElementById('traderChatBox').innerHTML = '';
            currentTrader = '';
        }

        function sendTraderMessage() {
            const input = document.getElementById('traderChatInput');
            const chatBox = document.getElementById('traderChatBox');
            if (input.value.trim()) {
                const message = document.createElement('div');
                message.className = 'chat-message sent';
                message.textContent = `You: ${input.value}`;
                chatBox.appendChild(message);
                chatBox.scrollTop = chatBox.scrollHeight;
                input.value = '';
                setTimeout(() => {
                    const reply = document.createElement('div');
                    reply.className = 'chat-message received';
                    reply.textContent = `${currentTrader}: Thanks for your message!`;
                    chatBox.appendChild(reply);
                    chatBox.scrollTop = chatBox.scrollHeight;
                }, 1000);
            }
}
function sendCoFundedMessage() {
            const input = document.getElementById('coFundedChatInput');
            const chatBox = document.getElementById('coFundedChatBox');
            if (input.value.trim()) {
                const message = document.createElement('div');
                message.className = 'chat-message sent';
                message.textContent = `You: ${input.value}`;
                chatBox.appendChild(message);
                chatBox.scrollTop = chatBox.scrollHeight;
                input.value = '';
            }
        }

        function sendSupportMessage() {
            const input = document.getElementById('supportChatInput');
            const chatBox = document.getElementById('supportChatBox');
            if (input.value.trim()) {
                const message = document.createElement('div');
                message.className = 'chat-message sent';
                message.textContent = `You: ${input.value}`;
                chatBox.appendChild(message);
                chatBox.scrollTop = chatBox.scrollHeight;
                input.value = '';
            }
        }

        function openTab(tabName) {
            document.querySelectorAll('#message-center .tab-
content').forEach(tab => {
                tab.classList.remove('active');
            });
            document.querySelectorAll('#message-center .tab-btn').forEach(btn => 
{
                btn.classList.remove('active');
            });
            document.getElementById(tabName).classList.add('active');
            document.querySelector(`button[onclick="openTab('$
{tabName}')"]`).classList.add('active');
        }

        function acceptRequest(requestId) {
            alert(`Request ${requestId} accepted!`);
        }

        function declineRequest(requestId) {
alert(`Request ${requestId} declined.`);
        }

        function viewRequestDetails(requestId) {
            alert(`Viewing details for request ${requestId}`);
        }

        function viewOrderDetails(orderId) {
            alert(`Viewing details for order ${orderId}`);
        }

        function fileDispute(orderId) {
            alert(`Filing dispute for order ${orderId}`);
        }

        function downloadAgreement(orderId) {
            alert(`Downloading agreement for order ${orderId}`);
        }

        function requestMatch(target) {
            alert(`Match request sent for ${target}!`);
        }

        function acceptMatch(matchId) {
            alert(`Match ${matchId} agreed and funded! Prop firm account 
purchase triggered.`);
        }

        // Form submission with validation
        document.querySelectorAll('form').forEach(form => {
            form.addEventListener('submit', async (e) => {
                e.preventDefault();
                const formId = form.id;
                const submitButton = form.querySelector('button[type="submit"]');
                submitButton.disabled = true;
                submitButton.classList.add('loading');
                submitButton.textContent = formId === 'deposit-form' ? 'Processing 
Deposit...' : 'Submitting...';

                // Clear previous error messages
                form.querySelectorAll('.error-message').forEach(el => el.remove());

                // Collect form data
                const formData = new FormData(form);
                const data = Object.fromEntries(formData);

                // Client-side validation
let isValid = true;
                for (const [key, value] of Object.entries(data)) {
                    if (!value && key !== 'certificate-file' && key !== 'amount-
description' && key !== 'deposit-note') {
                        isValid = false;
                        const field = form.querySelector(`[name="${key}"]`);
                        const error = document.createElement('p');
                        error.className = 'error-message';
                        error.textContent = `${key.replace(/-/g, ' ')} is required.`;
                        field.parentElement.appendChild(error);
                    }
                }

                if (formId === 'deposit-form' && data['deposit-amount'] && 
Number(data['deposit-amount']) < 10) {
                    isValid = false;
                    const field = form.querySelector('[name="deposit-amount"]');
                    const error = document.createElement('p');
                    error.className = 'error-message';
                    error.textContent = 'Deposit amount must be at least $10.';
                    field.parentElement.appendChild(error);
                }

                if (!isValid) {
                    submitButton.disabled = false;
                    submitButton.classList.remove('loading');
                    submitButton.textContent = formId === 'deposit-form' ? 'Submit 
Deposit' : 'Submit';
                    return;
                }

                try {
                    const response = await fetch('/api/submit-form', {
                        method: 'POST',
                        headers: { 'Content-Type': 'application/json' },
                        body: JSON.stringify({ formId, ...data }),
                    });

                    if (!response.ok) throw new Error('Submission failed');
                    const result = await response.json();
                    alert(`Form ${formId} submitted successfully!`);
                    form.reset();
                } catch (error) {
                    const errorMessage = document.createElement('p');
                    errorMessage.className = 'error-message';
                    errorMessage.textContent = 'Error submitting form. Please try 
again.';
form.appendChild(errorMessage);
                } finally {
                    submitButton.disabled = false;
                    submitButton.classList.remove('loading');
                    submitButton.textContent = formId === 'deposit-form' ? 'Submit 
Deposit' : 'Submit';
                }
            });
        });

        // Performance chart
        const ctx = 
document.getElementById('performanceChart')?.getContext('2d');
        if (ctx) {
            new Chart(ctx, {
                type: 'line',
                data: {
                    labels: ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul', 'Aug'],
                    datasets: [{
                        label: 'Profit/Loss (USD)',
                        data: [200, 400, 300, 600, 800, 500, 900, 1200],
                        borderColor: '#0a1f44',
                        backgroundColor: 'rgba(10, 31, 68, 0.1)',
                        fill: true,
                        tension: 0.4
                    }]
                },
                options: {
                    responsive: true,
                    scales: { y: { beginAtZero: true, title: { display: true, text: 'USD' } } }
                }
            });
        }

        // Initialize UI
        updateUI();
    </script>
</body>
</html>
