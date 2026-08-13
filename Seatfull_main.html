<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ClassKin - Attendance Tracking</title>

    <style>
        /* --- Custom Font Declaration --- */
        @font-face {
            font-family: 'Verona Serial';
            /* Pointing to a 'fonts' folder in the same directory as this HTML file */
            src: url('fonts/Verona-Serial-Regular.woff2') format('woff2'),
                 url('fonts/Verona-Serial-Regular.woff') format('woff'),
                 url('fonts/Verona-Serial-Regular.ttf') format('truetype'); /* Added TTF as a common fallback */
            font-weight: 400;
            font-style: normal;
            font-display: swap;
        }

        :root {
            --header-bg: #223c33;
            --bg-color: #f4f2e9;
            --card-bg: #ffffff;
            --text-main: #333333;
            --text-muted: #6b6b6b;
            --text-header: #c5c9c7;
            --accent-green: #487258;
            --banner-bg: #e6eee7;
            --border-light: #e5e1d8;
            
            /* Status Colors */
            --risk-high-bg: #fbe5e1;
            --risk-high-text: #d1563e;
            --risk-medium-bg: #fdf0df;
            --risk-medium-text: #b67843;
            --risk-low-bg: #ebf0ea;
            --risk-low-text: #2a7d4f;
            --success-text: #2a7d4f;
            --danger-text: #d1563e;
            
            /* Chart & Brand Colors */
            --brand-orange: #dcb36d;
            --chart-orange: #d1563e;
            --chart-green: #487258;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-main);
            min-height: 100vh;
            display: flex;
            flex-direction: column;
        }

        /* --- Global Title Font Rule --- */
        h1, h2, h3, h4, h5, h6 {
            font-family: 'Verona Serial', serif;
            font-weight: 400;
        }

        /* --- Login Screen Styling --- */
        #login-screen {
            display: flex;
            align-items: center;
            justify-content: center;
            height: 100vh;
            width: 100vw;
            background-color: var(--header-bg);
            position: fixed;
            top: 0;
            left: 0;
            z-index: 1000;
        }

        .login-card {
            background: var(--card-bg);
            padding: 40px;
            border-radius: 12px;
            width: 100%;
            max-width: 420px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.2);
            text-align: center;
        }

        .login-brand {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 12px;
            font-size: 1.8rem;
            font-weight: 600;
            font-family: 'Verona Serial', serif;
            color: var(--header-bg);
            margin-bottom: 8px;
        }

        .login-brand-icon {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 2px;
            width: 24px;
            height: 24px;
        }
        .login-brand-icon span {
            background-color: var(--brand-orange);
            border-radius: 50%;
            width: 10px;
            height: 10px;
        }

        .login-tagline { color: var(--text-muted); font-size: 0.95rem; margin-bottom: 32px; }
        .login-form-group { text-align: left; margin-bottom: 20px; }
        .login-form-group label { display: block; font-size: 0.85rem; font-weight: 600; color: var(--text-main); margin-bottom: 8px; }
        .login-form-group input { width: 100%; padding: 12px 14px; border: 1px solid var(--border-light); border-radius: 6px; font-size: 0.95rem; outline: none; transition: border-color 0.2s; background: #faf9f5;}
        .login-form-group input:focus { border-color: var(--accent-green); }

        .login-btn { width: 100%; padding: 14px; background-color: var(--accent-green); color: white; border: none; border-radius: 6px; font-size: 1rem; font-weight: 600; cursor: pointer; margin-top: 8px; transition: opacity 0.2s; }
        .login-btn:hover { opacity: 0.9; }
        .login-links { margin-top: 24px; font-size: 0.9rem; color: var(--text-muted); }
        .login-links a { color: var(--accent-green); text-decoration: none; }
        .login-divider { margin: 24px 0; border: 0; border-top: 1px solid var(--border-light); }
        .login-demo-info { font-size: 0.8rem; color: var(--text-muted); line-height: 1.6; }

        /* --- Main App Wrapper --- */
        #app-wrapper { display: none; flex-direction: column; min-height: 100vh; }

        /* --- Header Styling --- */
        .top-header {
            background-color: var(--header-bg);
            color: white;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 16px 32px;
        }

        .header-left { display: flex; align-items: center; gap: 24px; }
        .brand { 
            display: flex; 
            align-items: center; 
            gap: 10px; 
            font-size: 1.6rem; 
            font-weight: 600; 
            letter-spacing: 0.5px;
            font-family: 'Verona Serial', serif;
        }
        .brand-dots { display: grid; grid-template-columns: 1fr 1fr; gap: 2px; width: 16px; height: 16px; }
        .brand-dots span { background-color: var(--brand-orange); border-radius: 50%; width: 6px; height: 6px; }
        .header-divider { width: 1px; height: 32px; background-color: #3f554d; }
        
        .school-info { display: flex; flex-direction: column; gap: 2px; }
        .school-info .school-name { font-weight: 400; font-family: 'Times New Roman', serif; font-size: 1.1rem; }
        .school-info .district-name { font-size: 0.8rem; color: var(--text-header); }

        .header-right { display: flex; align-items: center; gap: 16px; font-size: 0.9rem; color: var(--text-header); }
        .btn-signout { background: transparent; color: white; border: 1px solid #486158; padding: 6px 12px; border-radius: 4px; cursor: pointer; transition: background 0.2s; }
        .btn-signout:hover { background: #2c4a3f; }

        /* --- Sub-Navigation Styling --- */
        .sub-nav {
            background-color: var(--bg-color);
            padding: 0 32px;
            display: flex;
            gap: 8px;
            box-shadow: inset 0 -1px 0 var(--border-light);
        }

        .nav-tab {
            padding: 16px 24px;
            cursor: pointer;
            color: var(--text-muted);
            font-size: 0.95rem;
            font-weight: 500;
            border-top: 3px solid transparent;
            background-color: transparent;
            border-radius: 4px 4px 0 0;
            transition: all 0.2s;
        }

        .nav-tab.active {
            background-color: var(--card-bg);
            color: var(--text-main);
            border-top-color: var(--accent-green);
            box-shadow: 0 -1px 0 var(--border-light), 1px 0 0 var(--border-light), -1px 0 0 var(--border-light);
        }

        /* --- Main Content Area --- */
        .main-content { flex-grow: 1; padding: 32px; max-width: 1400px; margin: 0 auto; width: 100%; }

        .welcome-banner { background-color: var(--banner-bg); color: var(--accent-green); padding: 18px 24px; border-radius: 6px; border-left: 4px solid var(--accent-green); margin-bottom: 32px; font-size: 1.05rem; }

        /* --- Cards & Grid --- */
        .stats-grid { display: grid; grid-template-columns: repeat(4, 1fr); gap: 24px; margin-bottom: 32px; }
        .card { background: var(--card-bg); border-radius: 8px; border: 1px solid var(--border-light); box-shadow: 0 2px 4px rgba(0,0,0,0.02); padding: 24px; margin-bottom: 24px; }
        .stat-title { font-family: 'Times New Roman', serif; font-weight: 600; font-size: 0.85rem; text-transform: uppercase; letter-spacing: 0.8px; color: var(--text-muted); margin-bottom: 16px; }
        .stat-value { font-size: 2.2rem; color: var(--text-main); margin-bottom: 12px; font-weight: 400; }
        .stat-value.success { color: var(--success-text); }
        .stat-value.danger { color: var(--danger-text); }
        .stat-desc { font-size: 0.85rem; color: var(--text-muted); }

        /* --- Shared Components & Lists --- */
        .card-title { font-family: 'Verona Serial', serif; font-weight: 400; font-size: 1.2rem; color: var(--text-main); margin-bottom: 16px; }
        .data-list { list-style: none; }
        .data-list li { display: flex; justify-content: space-between; padding: 12px 0; border-bottom: 1px solid var(--border-light); font-size: 0.9rem; }
        .data-list li:last-child { border-bottom: none; padding-bottom: 0; }
        .data-label { color: var(--text-muted); }
        .data-value { font-weight: 500; text-align: right; }

        /* --- Table Section --- */
        .table-header { display: flex; justify-content: space-between; align-items: center; margin-bottom: 24px; flex-wrap: wrap; gap: 15px; }
        .table-header h2 { font-family: 'Verona Serial', serif; font-weight: 400; font-size: 1.4rem; color: var(--text-main); }
        table { width: 100%; border-collapse: collapse; }
        th { text-align: left; padding: 12px 16px; font-size: 0.75rem; text-transform: uppercase; letter-spacing: 0.5px; color: var(--text-muted); border-bottom: 1px solid var(--border-light); }
        td { padding: 16px; border-bottom: 1px solid var(--border-light); font-size: 0.95rem; color: var(--text-main); }
        tr:last-child td { border-bottom: none; }
        tbody tr { cursor: pointer; transition: background-color 0.1s; }
        tbody tr:hover { background-color: #faf9f5; }
        .student-id { font-weight: 600; }

        /* --- Badges & Filters --- */
        .badge { padding: 4px 10px; border-radius: 12px; font-size: 0.8rem; font-weight: 600; display: inline-block; }
        .badge.low { background-color: var(--risk-low-bg); color: var(--risk-low-text); }
        .badge.medium { background-color: var(--risk-medium-bg); color: var(--risk-medium-text); }
        .badge.high { background-color: var(--risk-high-bg); color: var(--risk-high-text); }
        .badge.neutral { background-color: #e8ecec; color: #555; }

        .filter-buttons { display: flex; gap: 8px; }
        .filter-btn { padding: 6px 14px; border-radius: 20px; border: 1px solid var(--border-light); background: var(--card-bg); color: var(--text-muted); font-size: 0.85rem; cursor: pointer; transition: all 0.2s; }
        .filter-btn.active, .filter-btn:hover { background: var(--text-main); color: white; border-color: var(--text-main); }
        .empty-state { text-align: center; padding: 40px; color: var(--text-muted); font-style: italic; }

        /* --- Forms & Buttons --- */
        .form-section { margin-bottom: 32px; }
        .form-section-title { font-family: 'Verona Serial', serif; font-weight: 400; font-size: 1.2rem; color: var(--text-main); margin-bottom: 16px; border-bottom: 1px solid var(--border-light); padding-bottom: 8px; }
        .form-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 20px; }
        .form-group { display: flex; flex-direction: column; gap: 6px; }
        .form-group.full-width { grid-column: 1 / -1; }
        .form-label { font-size: 0.85rem; font-weight: 600; color: var(--text-main); }
        .form-hint { font-size: 0.75rem; color: var(--text-muted); font-weight: normal; margin-left: 4px; }
        .form-input, .form-select { padding: 10px 12px; border: 1px solid var(--border-light); border-radius: 6px; font-size: 0.95rem; color: var(--text-main); outline: none; transition: border-color 0.2s; background: #faf9f5; }
        .form-input:focus, .form-select:focus { border-color: var(--accent-green); }
        .checkbox-group-wrapper { display: grid; grid-template-columns: 1fr 1fr; gap: 16px; margin-top: 16px; }
        .checkbox-label { display: flex; align-items: center; gap: 8px; font-size: 0.9rem; font-weight: 500; color: var(--text-main); cursor: pointer; }
        .checkbox-label input[type="checkbox"] { width: 16px; height: 16px; accent-color: var(--accent-green); }

        .btn { padding: 10px 20px; border-radius: 6px; font-size: 0.95rem; font-weight: 600; cursor: pointer; border: none; transition: opacity 0.2s; display: inline-block;}
        .btn:hover { opacity: 0.9; }
        .btn-primary { background-color: var(--accent-green); color: white; }
        .btn-secondary { background-color: white; color: var(--text-main); border: 1px solid var(--border-light); }
        .btn-warning { background-color: #d1563e; color: white; } 

        /* --- Detail Specific Layouts --- */
        .detail-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 20px; margin-bottom: 20px; }
        .header-context { font-size: 0.75rem; text-transform: uppercase; letter-spacing: 0.5px; color: var(--accent-green); font-weight: bold; margin-bottom: 4px; }
        .score-row { display: flex; justify-content: space-between; font-size: 0.85rem; padding: 6px 0; color: var(--text-muted); }
        .score-row.total { border-top: 1px dashed var(--border-light); margin-top: 8px; padding-top: 12px; font-weight: bold; color: var(--text-main); }
        
        .funding-highlight { background-color: var(--bg-color); padding: 12px 16px; border-radius: 6px; margin-bottom: 20px; font-size: 0.95rem; border: 1px solid var(--border-light); }
        .funding-metrics { display: grid; grid-template-columns: repeat(3, 1fr); gap: 16px; }
        .funding-metric-box { border: 1px solid var(--border-light); border-radius: 8px; padding: 16px; }
        .fm-label { font-size: 0.75rem; text-transform: uppercase; color: var(--text-muted); margin-bottom: 8px; font-weight: 600; }
        .fm-value { font-size: 1.5rem; color: var(--text-main); font-weight: bold; margin-bottom: 4px; }
        .fm-value.success { color: var(--success-text); }
        .fm-desc { font-size: 0.8rem; color: var(--text-muted); }

        .progress-tracker { display: flex; gap: 4px; margin-bottom: 24px; }
        .progress-step { flex: 1; padding: 10px; text-align: center; font-size: 0.85rem; font-weight: 600; border-radius: 6px; background: var(--bg-color); color: var(--text-muted); border: 1px solid var(--border-light); }
        .progress-step.completed { background: var(--accent-green); color: white; border-color: var(--accent-green); }
        .progress-step.current { background: var(--text-main); color: white; border-color: var(--text-main); }

        .text-success { color: var(--success-text); font-weight: 600; }
        .text-danger { color: var(--danger-text); font-weight: 600; }

        /* View Switching Logic */
        #view-dashboard, #view-flag-student, #view-account, #view-student-detail, #view-subsidy, #view-financials { display: none; }
    </style>
</head>
<body>

    <div id="login-screen">
        <div class="login-card">
            <div class="login-brand">
                <div class="login-brand-icon">
                    <span></span><span></span>
                    <span></span><span></span>
                </div>
                ClassKin
            </div>
            <div class="login-tagline">Every seat full, every day.</div>

            <div class="login-form-group">
                <label>Work email</label>
                <input type="email" id="login-email" placeholder="maria@classkin.app" value="coordinator@classkin.app">
            </div>
            <div class="login-form-group">
                <label>Password</label>
                <input type="password" placeholder="••••••••" value="classkin123">
            </div>

            <button class="login-btn" onclick="doLogin()">Sign in</button>

            <div class="login-links">
                New here? <a href="#">Create an account</a>
            </div>

            <hr class="login-divider">

            <div class="login-demo-info">
                Demo accounts, password <strong>classkin123</strong><br>
                coordinator@classkin.app · finance@classkin.app
            </div>
        </div>
    </div>

    <div id="app-wrapper">
        <header class="top-header">
            <div class="header-left">
                <div class="brand">
                    <div class="brand-dots">
                        <span></span><span></span>
                        <span></span><span></span>
                    </div>
                    ClassKin
                </div>
                <div class="header-divider"></div>
                <div class="school-info">
                    <div class="school-name">Lincoln High School</div>
                    <div class="district-name">Jefferson County USD</div>
                </div>
            </div>
            <div class="header-right">
                <span class="user-info" id="user-info-text">Maria Coordinator • Coordinator</span>
                <button class="btn-signout" onclick="doLogout()">Sign out</button>
            </div>
        </header>

        <nav class="sub-nav" id="horizontal-nav">
            <div class="nav-tab active" data-target="view-dashboard">Dashboard</div>
            <div class="nav-tab" data-target="view-flag-student">Flag a student</div>
            <div class="nav-tab" id="nav-financials" data-target="view-financials" style="display: none;">Financials</div>
            <div class="nav-tab" data-target="view-account">Account</div>
        </nav>

        <main class="main-content">
            
            <div id="view-dashboard">
                <div class="welcome-banner" id="welcome-message">
                    Welcome back, Maria.
                </div>

                <div class="stats-grid">
                    <div class="card stat-card" style="margin: 0;">
                        <div class="stat-title">Students Flagged</div>
                        <div class="stat-value" id="stat-total">0</div>
                        <div class="stat-desc">Caregiving cause identified</div>
                    </div>
                    <div class="card stat-card" style="margin: 0;">
                        <div class="stat-title">High Risk</div>
                        <div class="stat-value danger" id="stat-high">0</div>
                        <div class="stat-desc">Score of 66 or above</div>
                    </div>
                    <div class="card stat-card" style="margin: 0;">
                        <div class="stat-title">Attendance Recovered</div>
                        <div class="stat-value">44%</div>
                        <div class="stat-desc">Matched to care or resolved</div>
                    </div>
                    <div class="card stat-card" style="margin: 0;">
                        <div class="stat-title">Funding Preserved</div>
                        <div class="stat-value success">$9,072</div>
                        <div class="stat-desc">Projected this term</div>
                    </div>
                </div>

                <div class="card table-section">
                    <div class="table-header">
                        <div style="display: flex; align-items: center; gap: 20px; flex-wrap: wrap;">
                            <h2>Flagged students</h2>
                            <div class="filter-buttons" id="filter-container">
                                <button class="filter-btn active" data-filter="all">All</button>
                                <button class="filter-btn" data-filter="high">High risk</button>
                                <button class="filter-btn" data-filter="subsidy">Needs subsidy action</button>
                                <button class="filter-btn" data-filter="care">Needs care match</button>
                            </div>
                        </div>
                        <span id="student-count" style="color: var(--text-muted); font-size: 0.9rem;"></span>
                    </div>
                    
                    <table>
                        <thead>
                            <tr>
                                <th>Student</th>
                                <th>Grade</th>
                                <th>Risk</th>
                                <th>Predicted Absences</th>
                                <th>Funding at Risk</th>
                                <th>Subsidy</th>
                                <th>Care</th>
                            </tr>
                        </thead>
                        <tbody id="student-table-body">
                            </tbody>
                    </table>
                </div>
            </div>

            <div id="view-flag-student">
                <div class="card form-container" style="max-width: 900px;">
                    <div class="form-section">
                        <h3 class="form-section-title">Student</h3>
                        <div class="form-grid">
                            <div class="form-group">
                                <label class="form-label">Anonymized code <span class="form-hint">No real names are stored</span></label>
                                <input type="text" class="form-input" value="STU-4821">
                            </div>
                            <div class="form-group">
                                <label class="form-label">Grade</label>
                                <input type="text" class="form-input" value="9">
                            </div>
                            <div class="form-group">
                                <label class="form-label">Income proxy</label>
                                <select class="form-select">
                                    <option>Unknown</option>
                                    <option>Free/Reduced Lunch</option>
                                </select>
                            </div>
                            <div class="form-group">
                                <label class="form-label">Household size</label>
                                <input type="text" class="form-input" value="4">
                            </div>
                            <div class="form-group">
                                <label class="form-label">Younger sibling age</label>
                                <input type="text" class="form-input" value="3">
                            </div>
                        </div>
                    </div>

                    <div class="form-section">
                        <h3 class="form-section-title">Caregiving</h3>
                        <div class="form-grid">
                            <div class="form-group full-width">
                                <label class="form-label">Why is this student being flagged?</label>
                                <input type="text" class="form-input" value="Sibling caregiving (counselor check-in)">
                            </div>
                        </div>
                        
                        <div class="checkbox-group-wrapper">
                            <label class="checkbox-label">
                                <input type="checkbox" checked> Caregiving is the suspected cause
                            </label>
                            <label class="checkbox-label">
                                <input type="checkbox"> A staff member confirmed it with the family
                            </label>
                            <label class="checkbox-label">
                                <input type="checkbox"> Family consent is on file
                            </label>
                        </div>
                    </div>

                    <div class="form-actions">
                        <button class="btn btn-primary">Flag and score student</button>
                        <button class="btn btn-secondary" onclick="switchToView('view-dashboard')">Cancel</button>
                    </div>
                </div>
            </div>

            <div id="view-account">
                <div class="card" style="max-width: 600px;">
                    <h3 class="card-title">Account Details</h3>
                    <p style="color: var(--text-muted); margin-bottom: 24px;">FERPA-aligned environment active. No real student names are stored.</p>
                    <ul class="data-list">
                        <li><span class="data-label">Name</span><span class="data-value" id="acc-name">Maria Coordinator</span></li>
                        <li><span class="data-label">Role</span><span class="data-value" id="acc-role">Coordinator</span></li>
                        <li><span class="data-label">School</span><span class="data-value">Lincoln High School</span></li>
                        <li><span class="data-label">District</span><span class="data-value">Jefferson County USD</span></li>
                    </ul>
                </div>
            </div>

            <div id="view-student-detail">
                <div style="display: flex; justify-content: space-between; align-items: flex-start; margin-bottom: 24px;">
                    <div>
                        <div class="header-context">Lincoln High School</div>
                        <h2 id="sd-id" style="font-size: 2.2rem; font-family: 'Verona Serial', serif; font-weight: 400; margin-bottom: 12px;">STU-4801</h2>
                        <div style="display: flex; align-items: center; gap: 12px; font-size: 0.9rem; color: var(--text-muted);">
                            <span id="sd-grade">Grade 10</span> &bull; 
                            <span id="sd-badge-risk" class="badge medium">Medium risk - 60</span>
                            <span class="badge neutral">Flagged</span>
                        </div>
                    </div>
                    <button class="btn btn-secondary" onclick="switchToView('view-dashboard')">Back to dashboard</button>
                </div>

                <div class="card">
                    <h3 class="card-title">Why this student is flagged</h3>
                    <p id="sd-cause" style="font-size: 0.95rem; margin-bottom: 20px; color: var(--text-main);">Sibling caregiving (counselor check-in)</p>
                    <ul class="data-list">
                        <li><span class="data-label">Caregiving cause</span><span class="data-value">Confirmed by staff</span></li>
                        <li><span class="data-label">Family consent</span><span class="data-value">On file</span></li>
                        <li><span class="data-label">Younger sibling</span><span class="data-value" id="sd-sibling">3 years old</span></li>
                        <li><span class="data-label">Household size</span><span class="data-value" id="sd-household">5</span></li>
                    </ul>
                </div>

                <div class="detail-grid">
                    <div class="card" style="margin-bottom: 0;">
                        <h3 class="card-title">Attendance and prediction</h3>
                        <ul class="data-list" style="margin-bottom: 20px;">
                            <li><span class="data-label">School days so far</span><span class="data-value">90</span></li>
                            <li><span class="data-label">Absences</span><span class="data-value" id="sd-absences">14</span></li>
                            <li><span class="data-label">Tardies</span><span class="data-value" id="sd-tardies">8</span></li>
                            <li><span class="data-label">Early dismissals</span><span class="data-value" id="sd-early">6</span></li>
                            <li><span class="data-label">Last 30 days</span><span class="data-value" id="sd-recent">7 absences</span></li>
                        </ul>
                        <div style="background-color: var(--bg-color); padding: 12px 16px; border-radius: 6px; border: 1px solid var(--border-light); font-size: 0.9rem;">
                            Predicted <strong id="sd-pred-days">28 more absences</strong> over the rest of the term.
                        </div>
                    </div>

                    <div class="card" style="margin-bottom: 0;">
                        <h3 class="card-title">How the score was reached</h3>
                        <p style="font-size: 0.85rem; color: var(--text-muted); margin-bottom: 16px;">A transparent rules-based model. Every point is traceable.</p>
                        <div class="score-row"><span>Absence rate (<span id="sd-abs-rate">31%</span>)</span><span id="sd-pts-abs">14.0 pts</span></div>
                        <div class="score-row"><span>Recent pace (7 in 30 days)</span><span id="sd-pts-recent">21.9 pts</span></div>
                        <div class="score-row"><span>First or last period clustering</span><span id="sd-pts-cluster">14.4 pts</span></div>
                        <div class="score-row"><span>Caregiving confirmed by staff</span><span>10 pts</span></div>
                        <div class="score-row total"><span>Total</span><span id="sd-score-total">60 / 100</span></div>
                    </div>
                </div>

                <div class="card">
                    <h3 class="card-title">Funding at risk</h3>
                    <p style="font-size: 0.85rem; color: var(--text-muted); margin-bottom: 16px;">Attendance-funded district. Every missed day is money the district does not receive.</p>
                    <div class="funding-highlight">
                        <span id="sd-fund-calc-days">28</span> predicted days &times; $45 per day = <strong id="sd-fund-total">$1,260 at risk</strong>
                    </div>
                    <div class="funding-metrics">
                        <div class="funding-metric-box">
                            <div class="fm-label">Recoverable</div>
                            <div class="fm-value success" id="sd-fund-rec">$882</div>
                            <div class="fm-desc">If attendance is restored</div>
                        </div>
                        <div class="funding-metric-box">
                            <div class="fm-label">District Cost</div>
                            <div class="fm-value">$40</div>
                            <div class="fm-desc">Admin fee only, subsidy covers care</div>
                        </div>
                        <div class="funding-metric-box">
                            <div class="fm-label">Net to District</div>
                            <div class="fm-value success" id="sd-fund-net">$842</div>
                            <div class="fm-desc">Recoverable minus cost</div>
                        </div>
                    </div>
                </div>

                <div class="detail-grid">
                    <div class="card" style="margin-bottom: 0;">
                        <h3 class="card-title">Childcare subsidy</h3>
                        <ul class="data-list" style="margin-bottom: 24px;">
                            <li><span class="data-label">Program</span><span class="data-value">CCAP (Child Care Assistance Program)</span></li>
                            <li><span class="data-label">Eligibility</span><span class="data-value">Eligible</span></li>
                            <li><span class="data-label">Estimated benefit</span><span class="data-value">$1,200</span></li>
                            <li><span class="data-label">Status</span><span class="data-value" id="sd-sub-status">Applied</span></li>
                        </ul>
                        <button class="btn btn-primary" id="sd-sub-btn">Continue application</button>
                    </div>
                    
                    <div class="card" style="margin-bottom: 0;">
                        <h3 class="card-title">Care placement</h3>
                        <p style="font-size: 0.9rem; color: var(--text-main); margin-bottom: 24px; line-height: 1.5;" id="sd-care-desc">
                            No licensed provider matched yet for the younger sibling.
                        </p>
                        <button class="btn btn-secondary" id="sd-care-btn">Match care</button>
                    </div>
                </div>
            </div>

            <div id="view-subsidy">
                <div style="display: flex; justify-content: space-between; align-items: flex-start; margin-bottom: 24px;">
                    <div>
                        <div class="header-context" id="sub-header-context">STU-4801 • GRADE 10</div>
                        <h2 style="font-size: 2rem; font-family: 'Verona Serial', serif; font-weight: 400; margin-bottom: 8px;">Childcare subsidy</h2>
                        <p style="color: var(--text-muted); font-size: 0.95rem;">Most of these families already qualify. The barrier is the paperwork, not the eligibility.</p>
                    </div>
                    <button class="btn btn-secondary" id="btn-back-student">Back to student</button>
                </div>

                <div class="card">
                    <h3 class="card-title">Application status</h3>
                    <div class="progress-tracker">
                        <div class="progress-step completed">Screening</div>
                        <div class="progress-step current">Applied</div>
                        <div class="progress-step">Approved</div>
                        <div class="progress-step">Care active</div>
                    </div>
                    
                    <ul class="data-list" style="margin-bottom: 24px;">
                        <li><span class="data-label">Program</span><span class="data-value">CCAP (Child Care Assistance Program)</span></li>
                        <li><span class="data-label">Screening result</span><span class="data-value">Eligible</span></li>
                        <li><span class="data-label">Estimated benefit</span><span class="data-value">$1,200 per term</span></li>
                    </ul>

                    <div style="display: flex; align-items: center; gap: 16px;">
                        <button class="btn btn-warning">Advance to approved</button>
                        <span style="font-size: 0.85rem; color: var(--text-muted);">Demo control. A live build would sync status from the state agency.</span>
                    </div>
                </div>

                <div class="card">
                    <h3 class="card-title">Update the household details</h3>
                    <p style="font-size: 0.85rem; color: var(--text-muted); margin-bottom: 20px;">Ask the family these four things. The app checks every program at once.</p>
                    
                    <div class="form-grid" style="margin-bottom: 24px;">
                        <div class="form-group">
                            <label class="form-label">How many people live in the home?</label>
                            <input type="text" class="form-input" id="sub-household" value="5">
                        </div>
                        <div class="form-group">
                            <label class="form-label">Monthly household income</label>
                            <select class="form-select">
                                <option>$2,500 - $3,500</option>
                                <option>Under $2,500</option>
                                <option>$3,500 - $4,500</option>
                            </select>
                        </div>
                        <div class="form-group">
                            <label class="form-label">How many children?</label>
                            <input type="text" class="form-input" value="2">
                        </div>
                        <div class="form-group">
                            <label class="form-label">Parent work schedule</label>
                            <input type="text" class="form-input" value="Weekday early shift">
                        </div>
                    </div>
                    
                    <button class="btn btn-primary">Check eligibility and submit</button>
                </div>
            </div>

            <div id="view-financials">
                <h2 style="font-size: 2rem; font-family: 'Verona Serial', serif; font-weight: 400; margin-bottom: 8px;">Financials</h2>
                <p style="color: var(--text-muted); margin-bottom: 24px;">Jefferson County USD - Attendance-funded district</p>

                <div style="background-color: var(--header-bg); padding: 30px; border-radius: 12px; margin-bottom: 24px; box-shadow: 0 4px 12px rgba(0,0,0,0.1);">
                    <div style="font-size: 0.75rem; color: var(--text-header); text-transform: uppercase; letter-spacing: 0.5px; font-weight: bold; margin-bottom: 8px;">Net district gain this term</div>
                    <div style="font-size: 3.5rem; font-weight: bold; color: white; line-height: 1;">$5,236</div>
                    <div style="font-size: 0.9rem; color: var(--text-header); margin-top: 12px;">Recoverable funding minus what the district spends to recover it.</div>
                </div>

                <div class="stats-grid">
                    <div class="card stat-card" style="margin:0;">
                        <div class="stat-title">Funding At Risk</div>
                        <div class="stat-value" style="font-size: 2rem;">$16,965</div>
                        <div class="stat-desc">Projected from predicted absences</div>
                    </div>
                    <div class="card stat-card" style="margin:0;">
                        <div class="stat-title">Recoverable</div>
                        <div class="stat-value success" style="font-size: 2rem;">$11,876</div>
                        <div class="stat-desc">At a 70% recovery rate</div>
                    </div>
                    <div class="card stat-card" style="margin:0;">
                        <div class="stat-title">Subsidy Unlocked</div>
                        <div class="stat-value" style="font-size: 2rem;">$19,200</div>
                        <div class="stat-desc">Paid by programs, not the district</div>
                    </div>
                    <div class="card stat-card" style="margin:0;">
                        <div class="stat-title">District Cost</div>
                        <div class="stat-value" style="font-size: 2rem;">$6,640</div>
                        <div class="stat-desc">Admin fees plus uncovered care</div>
                    </div>
                </div>

                <div class="card" style="padding: 0; margin-bottom: 60px;">
                    <div style="padding: 24px 24px 16px 24px;">
                        <h3 class="card-title" style="margin: 0;">Return by student</h3>
                    </div>
                    <table style="width: 100%; margin-bottom: 0;">
                        <thead>
                            <tr>
                                <th>Student</th>
                                <th>Risk</th>
                                <th>Funding at Risk</th>
                                <th>Recoverable</th>
                                <th>District Cost</th>
                                <th>Net</th>
                            </tr>
                        </thead>
                        <tbody style="border-bottom: none;">
                            <tr><td class="student-id">STU-4801</td><td><span class="badge medium">Medium</span></td><td>$1,260</td><td>$882</td><td>$40</td><td class="text-success">$842</td></tr>
                            <tr><td class="student-id">STU-4802</td><td><span class="badge medium">Medium</span></td><td>$1,260</td><td>$882</td><td>$40</td><td class="text-success">$842</td></tr>
                            <tr><td class="student-id">STU-4804</td><td><span class="badge medium">Medium</span></td><td>$1,260</td><td>$882</td><td>$40</td><td class="text-success">$842</td></tr>
                            <tr><td class="student-id">STU-4807</td><td><span class="badge medium">Medium</span></td><td>$1,260</td><td>$882</td><td>$40</td><td class="text-success">$842</td></tr>
                            <tr><td class="student-id">STU-4810</td><td><span class="badge medium">Medium</span></td><td>$1,260</td><td>$882</td><td>$40</td><td class="text-success">$842</td></tr>
                            <tr><td class="student-id">STU-4803</td><td><span class="badge medium">Medium</span></td><td>$675</td><td>$472</td><td>$40</td><td class="text-success">$432</td></tr>
                            <tr><td class="student-id">STU-4805</td><td><span class="badge low">Low</span></td><td>$225</td><td>$158</td><td>$1,200</td><td class="text-danger">$-1,042</td></tr>
                            <tr><td class="student-id">STU-4809</td><td><span class="badge low">Low</span></td><td>$225</td><td>$158</td><td>$1,200</td><td class="text-danger">$-1,042</td></tr>
                            <tr><td class="student-id">STU-4821</td><td><span class="badge low">Low</span></td><td>$0</td><td>$0</td><td>$1,200</td><td class="text-danger">$-1,200</td></tr>
                        </tbody>
                    </table>
                </div>
            </div>

        </main>
    </div>

    <script>
        // --- 0. AUTH & ROLE LOGIC ---
        function doLogin() {
            const emailInput = document.getElementById('login-email').value.trim().toLowerCase();
            
            // Set Role Specific UI
            if (emailInput === 'finance@classkin.app') {
                document.getElementById('nav-financials').style.display = 'block';
                document.getElementById('user-info-text').textContent = 'Finance Admin • Finance';
                document.getElementById('acc-name').textContent = 'Finance Admin';
                document.getElementById('acc-role').textContent = 'Finance';
                document.getElementById('welcome-message').textContent = 'Welcome back, Finance Admin.';
            } else {
                document.getElementById('nav-financials').style.display = 'none';
                document.getElementById('user-info-text').textContent = 'Maria Coordinator • Coordinator';
                document.getElementById('acc-name').textContent = 'Maria Coordinator';
                document.getElementById('acc-role').textContent = 'Coordinator';
                document.getElementById('welcome-message').textContent = 'Welcome back, Maria.';
            }

            // Hide Login / Show App
            document.getElementById('login-screen').style.display = 'none';
            document.getElementById('app-wrapper').style.display = 'flex';
            
            // Navigate to default view
            if(emailInput === 'finance@classkin.app') {
                switchToView('view-financials');
            } else {
                switchToView('view-dashboard');
                initStats();
                renderTable(dummyData);
            }
        }

        function doLogout() {
            document.getElementById('login-screen').style.display = 'flex';
            document.getElementById('app-wrapper').style.display = 'none';
        }

        // --- 1. NAVIGATION LOGIC ---
        const navTabs = document.querySelectorAll('#horizontal-nav .nav-tab');
        const views = {
            'view-dashboard': document.getElementById('view-dashboard'),
            'view-flag-student': document.getElementById('view-flag-student'),
            'view-account': document.getElementById('view-account'),
            'view-student-detail': document.getElementById('view-student-detail'),
            'view-subsidy': document.getElementById('view-subsidy'),
            'view-financials': document.getElementById('view-financials')
        };

        function switchToView(targetId) {
            Object.values(views).forEach(view => {
                if(view) view.style.display = 'none';
            });
            
            if (views[targetId]) {
                views[targetId].style.display = 'block';
            }

            navTabs.forEach(tab => {
                if (tab.getAttribute('data-target') === targetId) {
                    tab.classList.add('active');
                } else {
                    tab.classList.remove('active');
                }
            });

            // Clear sub-nav active state if on a detail page
            if (targetId === 'view-student-detail' || targetId === 'view-subsidy') {
                navTabs.forEach(tab => tab.classList.remove('active'));
            }
        }

        navTabs.forEach(tab => {
            tab.addEventListener('click', () => {
                const target = tab.getAttribute('data-target');
                switchToView(target);
            });
        });


        // --- 2. DATA LOGIC ---
        let currentStudentId = null;

        const dummyData = [
            { id: "STU-4801", grade: 10, riskScore: 60, days: 28, funding: 1260, subsidy: "Applied", care: "None", absences: 14, tardies: 8, earlyDismissals: 6, recentAbsences: 7, siblingAge: "3 years old", householdSize: 5 },
            { id: "STU-4802", grade: 11, riskScore: 60, days: 28, funding: 1260, subsidy: "Approved", care: "Sunrise Learning Center", absences: 12, tardies: 2, earlyDismissals: 1, recentAbsences: 4, siblingAge: "4 years old", householdSize: 4 },
            { id: "STU-4805", grade: 10, riskScore: 78, days: 36, funding: 1620, subsidy: "Action needed", care: "None", absences: 20, tardies: 12, earlyDismissals: 4, recentAbsences: 9, siblingAge: "2 years old", householdSize: 6 },
            { id: "STU-4804", grade: 12, riskScore: 60, days: 28, funding: 1260, subsidy: "Care active", care: "Sunrise Learning Center", absences: 13, tardies: 5, earlyDismissals: 2, recentAbsences: 5, siblingAge: "1 year old", householdSize: 3 },
            { id: "STU-4807", grade: 11, riskScore: 60, days: 28, funding: 1260, subsidy: "Approved", care: "Sunrise Learning Center", absences: 15, tardies: 4, earlyDismissals: 0, recentAbsences: 6, siblingAge: "4 years old", householdSize: 5 },
            { id: "STU-4808", grade: 9,  riskScore: 71, days: 32, funding: 1440, subsidy: "Applied", care: "None", absences: 18, tardies: 9, earlyDismissals: 5, recentAbsences: 8, siblingAge: "8 months old", householdSize: 4 },
            { id: "STU-4812", grade: 9,  riskScore: 60, days: 28, funding: 1260, subsidy: "Care active", care: "Sunrise Learning Center", absences: 11, tardies: 6, earlyDismissals: 3, recentAbsences: 4, siblingAge: "3 years old", householdSize: 6 },
            { id: "STU-4817", grade: 10, riskScore: 60, days: 28, funding: 1260, subsidy: "Applied", care: "None", absences: 14, tardies: 7, earlyDismissals: 4, recentAbsences: 6, siblingAge: "2 years old", householdSize: 4 },
            { id: "STU-4803", grade: 9,  riskScore: 40, days: 15, funding: 675, subsidy: "Action needed", care: "None", absences: 8, tardies: 3, earlyDismissals: 1, recentAbsences: 2, siblingAge: "4 years old", householdSize: 3 },
            { id: "STU-4806", grade: 10, riskScore: 40, days: 15, funding: 675, subsidy: "Applied", care: "None", absences: 9, tardies: 2, earlyDismissals: 2, recentAbsences: 3, siblingAge: "3 years old", householdSize: 4 }
        ];

        const formatMoney = (amount) => new Intl.NumberFormat('en-US', { style: 'currency', currency: 'USD', maximumFractionDigits: 0 }).format(amount);

        function renderTable(data) {
            const tableBody = document.getElementById("student-table-body");
            const studentCount = document.getElementById("student-count");
            
            tableBody.innerHTML = ""; 
            const sortedData = [...data].sort((a, b) => b.riskScore - a.riskScore);

            if (sortedData.length === 0) {
                tableBody.innerHTML = `<tr><td colspan="7" class="empty-state">No students match this filter.</td></tr>`;
                studentCount.textContent = `0 shown`;
                return;
            }
            
            sortedData.forEach(student => {
                const row = document.createElement("tr");
                const riskLevel = student.riskScore >= 66 ? 'High' : 'Medium';
                const badgeClass = student.riskScore >= 66 ? 'high' : 'medium';

                row.innerHTML = `
                    <td class="student-id">${student.id}</td>
                    <td>${student.grade}</td>
                    <td><span class="badge ${badgeClass}">${riskLevel} ${student.riskScore}</span></td>
                    <td>${student.days} days</td>
                    <td>${formatMoney(student.funding)}</td>
                    <td>${student.subsidy}</td>
                    <td>${student.care}</td>
                `;
                
                row.addEventListener('click', () => openStudentDetail(student.id));
                tableBody.appendChild(row);
            });
            studentCount.textContent = `${sortedData.length} shown`;
        }

        function initStats() {
            document.getElementById("stat-total").textContent = dummyData.length;
            const highRiskCount = dummyData.filter(s => s.riskScore >= 66).length;
            document.getElementById("stat-high").textContent = highRiskCount;
        }

        document.getElementById("filter-container").addEventListener("click", function(e) {
            if (e.target.tagName === "BUTTON") {
                document.querySelectorAll(".filter-btn").forEach(btn => btn.classList.remove("active"));
                e.target.classList.add("active");

                const filterType = e.target.getAttribute("data-filter");
                let filteredData = dummyData;
                
                if (filterType === "high") {
                    filteredData = dummyData.filter(s => s.riskScore >= 66);
                } else if (filterType === "subsidy") {
                    filteredData = dummyData.filter(s => s.subsidy === "Action needed" || s.subsidy === "Applied");
                } else if (filterType === "care") {
                    filteredData = dummyData.filter(s => s.care === "None");
                }
                renderTable(filteredData);
            }
        });


        // --- 3. STUDENT DETAIL LOGIC ---
        function openStudentDetail(studentId) {
            const student = dummyData.find(s => s.id === studentId);
            if(!student) return;

            currentStudentId = studentId;

            document.getElementById('sd-id').textContent = student.id;
            document.getElementById('sd-grade').textContent = `Grade ${student.grade}`;
            
            const riskBadge = document.getElementById('sd-badge-risk');
            if(student.riskScore >= 66) {
                riskBadge.className = 'badge high';
                riskBadge.textContent = `High risk - ${student.riskScore}`;
            } else {
                riskBadge.className = 'badge medium';
                riskBadge.textContent = `Medium risk - ${student.riskScore}`;
            }

            document.getElementById('sd-sibling').textContent = student.siblingAge;
            document.getElementById('sd-household').textContent = student.householdSize;
            document.getElementById('sd-absences').textContent = student.absences;
            document.getElementById('sd-tardies').textContent = student.tardies;
            document.getElementById('sd-early').textContent = student.earlyDismissals;
            document.getElementById('sd-recent').textContent = `${student.recentAbsences} absences`;
            document.getElementById('sd-pred-days').textContent = `${student.days} more absences`;
            
            const baseAbsRate = Math.round((student.absences / 90) * 100);
            document.getElementById('sd-abs-rate').textContent = `${baseAbsRate}%`;
            document.getElementById('sd-pts-abs').textContent = `${(baseAbsRate * 0.45).toFixed(1)} pts`;
            document.getElementById('sd-pts-recent').textContent = `${(student.recentAbsences * 3.1).toFixed(1)} pts`;
            
            let calculatedPts = (baseAbsRate * 0.45) + (student.recentAbsences * 3.1) + 10;
            let clusterPts = student.riskScore - calculatedPts;
            if(clusterPts < 0) clusterPts = 2.4; 
            
            document.getElementById('sd-pts-cluster').textContent = `${clusterPts.toFixed(1)} pts`;
            document.getElementById('sd-score-total').textContent = `${student.riskScore} / 100`;

            document.getElementById('sd-fund-calc-days').textContent = student.days;
            document.getElementById('sd-fund-total').innerHTML = `<strong>${formatMoney(student.funding)} at risk</strong>`;
            
            const recoverable = student.funding * 0.70;
            const net = recoverable - 40;
            document.getElementById('sd-fund-rec').textContent = formatMoney(recoverable);
            document.getElementById('sd-fund-net').textContent = formatMoney(net);

            document.getElementById('sd-sub-status').textContent = student.subsidy;
            const subBtn = document.getElementById('sd-sub-btn');
            
            if(student.subsidy === 'Approved' || student.subsidy === 'Care active') {
                subBtn.style.display = 'none';
            } else {
                subBtn.style.display = 'inline-block';
                subBtn.textContent = student.subsidy === 'Action needed' ? 'Start application' : 'Continue application';
                subBtn.onclick = () => openSubsidyDetail(student.id);
            }

            const careDesc = document.getElementById('sd-care-desc');
            const careBtn = document.getElementById('sd-care-btn');
            
            if(student.care === "None") {
                careDesc.textContent = "No licensed provider matched yet for the younger sibling.";
                careBtn.style.display = 'inline-block';
            } else {
                careDesc.innerHTML = `Matched provider: <strong>${student.care}</strong>. Care is currently active and arranged.`;
                careBtn.style.display = 'none';
            }

            switchToView('view-student-detail');
        }

        // --- 4. SUBSIDY DETAIL LOGIC ---
        function openSubsidyDetail(studentId) {
            const student = dummyData.find(s => s.id === studentId);
            if(!student) return;

            document.getElementById('sub-header-context').textContent = `${student.id} • GRADE ${student.grade}`;
            document.getElementById('sub-household').value = student.householdSize || 5;

            switchToView('view-subsidy');
        }

        document.getElementById('btn-back-student').addEventListener('click', () => {
            if (currentStudentId) {
                openStudentDetail(currentStudentId);
            } else {
                switchToView('view-dashboard');
            }
        });

    </script>
</body>
</html>
