<!DOCTYPE html>
<html lang="hi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Smart Study Buddy - All Streams</title>
    <style>
        :root {
            --color-primary: #2180a1;
            --color-primary-hover: #1d7490;
            --color-secondary: #8b5cf6;
            --color-success: #22c55e;
            --color-danger: #c01517;
            --color-bg: #f5f5f5;
            --color-surface: #ffffff;
            --color-text: #1f2121;
            --color-text-secondary: #626c7c;
            --color-border: #e5e7eb;
            --space-8: 8px;
            --space-12: 12px;
            --space-16: 16px;
            --space-20: 20px;
            --space-24: 24px;
            --radius-base: 8px;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
            background: linear-gradient(135deg, #f5f5f5 0%, #e8f4f8 100%);
            color: var(--color-text);
            line-height: 1.5;
        }

        .ad-banner-top {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: var(--space-16);
            text-align: center;
            font-size: 13px;
            margin-bottom: var(--space-16);
            border-radius: var(--radius-base);
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: var(--space-16);
        }

        header {
            background: var(--color-surface);
            padding: var(--space-20);
            border-radius: var(--radius-base);
            margin-bottom: var(--space-20);
            box-shadow: 0 2px 8px rgba(33, 128, 161, 0.1);
            border-left: 5px solid var(--color-secondary);
        }

        h1 {
            font-size: 28px;
            margin-bottom: var(--space-8);
            color: var(--color-primary);
        }

        .header-subtitle {
            color: var(--color-text-secondary);
            font-size: 14px;
        }

        .tabs {
            display: flex;
            gap: var(--space-8);
            margin-bottom: var(--space-20);
            flex-wrap: wrap;
        }

        .tab-btn {
            padding: var(--space-12) var(--space-16);
            border: 2px solid var(--color-border);
            background: var(--color-surface);
            color: var(--color-text);
            border-radius: var(--radius-base);
            cursor: pointer;
            font-size: 14px;
            font-weight: 500;
            transition: all 0.3s;
        }

        .tab-btn.active {
            background: var(--color-primary);
            color: white;
            border-color: var(--color-primary);
        }

        .tab-btn:hover {
            border-color: var(--color-primary);
        }

        .tab-content {
            display: none;
        }

        .tab-content.active {
            display: block;
        }

        .form-group {
            margin-bottom: var(--space-16);
        }

        label {
            display: block;
            margin-bottom: var(--space-8);
            font-weight: 500;
            color: var(--color-text);
        }

        input, select, textarea {
            width: 100%;
            padding: var(--space-12);
            border: 1px solid var(--color-border);
            border-radius: var(--radius-base);
            font-size: 14px;
            font-family: inherit;
        }

        input:focus, select:focus, textarea:focus {
            outline: none;
            border-color: var(--color-primary);
            box-shadow: 0 0 0 3px rgba(33, 128, 161, 0.1);
        }

        .btn {
            padding: var(--space-12) var(--space-20);
            border: none;
            border-radius: var(--radius-base);
            cursor: pointer;
            font-size: 14px;
            font-weight: 600;
            transition: all 0.3s;
        }

        .btn-primary {
            background: var(--color-primary);
            color: white;
        }

        .btn-primary:hover {
            background: var(--color-primary-hover);
        }

        .btn-secondary {
            background: var(--color-border);
            color: var(--color-text);
        }

        .btn-secondary:hover {
            background: #d1d5db;
        }

        .card-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: var(--space-16);
            margin-bottom: var(--space-20);
        }

        .card {
            background: var(--color-surface);
            padding: var(--space-16);
            border-radius: var(--radius-base);
            border: 2px solid var(--color-border);
            transition: all 0.3s;
        }

        .card:hover {
            border-color: var(--color-primary);
            box-shadow: 0 4px 12px rgba(33, 128, 161, 0.15);
        }

        .card h3 {
            color: var(--color-primary);
            margin-bottom: var(--space-12);
            font-size: 16px;
        }

        .progress-bar {
            width: 100%;
            height: 8px;
            background: var(--color-border);
            border-radius: 4px;
            overflow: hidden;
            margin: var(--space-12) 0;
        }

        .progress-fill {
            height: 100%;
            background: linear-gradient(90deg, var(--color-primary), var(--color-success));
            transition: width 0.3s;
        }

        .stats {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: var(--space-16);
            margin-bottom: var(--space-20);
        }

        .stat-box {
            background: var(--color-surface);
            padding: var(--space-16);
            border-radius: var(--radius-base);
            text-align: center;
            border: 2px solid var(--color-border);
            border-left: 5px solid var(--color-secondary);
        }

        .stat-value {
            font-size: 28px;
            font-weight: bold;
            color: var(--color-primary);
            margin-bottom: var(--space-8);
        }

        .stat-label {
            font-size: 12px;
            color: var(--color-text-secondary);
            text-transform: uppercase;
        }

        .item-card {
            background: var(--color-surface);
            padding: var(--space-16);
            border-radius: var(--radius-base);
            margin-bottom: var(--space-12);
            border-left: 4px solid var(--color-primary);
            box-shadow: 0 1px 3px rgba(0,0,0,0.05);
        }

        .item-card h4 {
            color: var(--color-primary);
            margin-bottom: var(--space-8);
        }

        .item-card .meta {
            font-size: 12px;
            color: var(--color-text-secondary);
            margin-bottom: var(--space-8);
        }

        .ad-banner-side {
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            color: white;
            padding: var(--space-16);
            border-radius: var(--radius-base);
            text-align: center;
            margin-bottom: var(--space-16);
            font-size: 13px;
        }

        .setup-box {
            background: linear-gradient(135deg, var(--color-secondary) 0%, #7c3aed 100%);
            color: white;
            padding: var(--space-24);
            border-radius: var(--radius-base);
            text-align: center;
            margin-bottom: var(--space-20);
        }

        .setup-box h2 {
            color: white;
            margin-bottom: var(--space-12);
        }

        .setup-options {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: var(--space-12);
            margin: var(--space-20) 0;
        }

        .setup-option {
            background: rgba(255,255,255,0.1);
            padding: var(--space-16);
            border-radius: var(--radius-base);
            cursor: pointer;
            transition: all 0.3s;
            border: 2px solid transparent;
        }

        .setup-option:hover {
            background: rgba(255,255,255,0.2);
            border-color: white;
        }

        .setup-option.selected {
            background: white;
            color: var(--color-primary);
            border-color: var(--color-primary);
        }

        @media (max-width: 768px) {
            h1 {
                font-size: 22px;
            }

            .card-grid {
                grid-template-columns: 1fr;
            }

            .tabs {
                flex-direction: column;
            }

            .tab-btn {
                width: 100%;
            }
        }
    </style>
</head>
<body>
    <div class="ad-banner-top">
        📢 विज्ञापन | Smart Study Buddy - सभी Students के लिए!
    </div>

    <div class="container">
        <header>
            <h1>🧠 Smart Study Buddy</h1>
            <p class="header-subtitle">Class 10-12 सभी Streams | Personalized Study + Motivation 🔱</p>
        </header>

        <!-- Setup Section (First Time) -->
        <div id="setupSection" class="setup-box">
            <h2>🎯 अपना Setup करो</h2>
            <p style="margin-bottom: var(--space-16);">पहले अपना Class और Stream select करो</p>
            
            <div style="margin-bottom: var(--space-16);">
                <label style="color: white; margin-bottom: var(--space-8);">Class:</label>
                <div class="setup-options">
                    <div class="setup-option" onclick="selectClass('10th')">10th</div>
                    <div class="setup-option selected" onclick="selectClass('12th')">12th</div>
                </div>
            </div>

            <div id="streamOptions" style="margin-bottom: var(--space-16);">
                <label style="color: white; margin-bottom: var(--space-8);">Stream:</label>
                <div class="setup-options">
                    <div class="setup-option selected" onclick="selectStream('PCB')">PCB</div>
                    <div class="setup-option" onclick="selectStream('PCM')">PCM</div>
                    <div class="setup-option" onclick="selectStream('PCA')">PCA</div>
                    <div class="setup-option" onclick="selectStream('Commerce')">Commerce</div>
                    <div class="setup-option" onclick="selectStream('Arts')">Arts</div>
                </div>
            </div>

            <button class="btn btn-primary" onclick="completeSetup()">✅ Continue</button>
        </div>

        <!-- Main Tabs -->
        <div class="tabs" id="mainTabs" style="display: none;">
            <button class="tab-btn active" onclick="switchTab('dashboard')">📊 Dashboard</button>
            <button class="tab-btn" onclick="switchTab('planner')">📅 Planner</button>
            <button class="tab-btn" onclick="switchTab('notes')">📝 Notes</button>
            <button class="tab-btn" onclick="switchTab('motivation')">💪 Motivation</button>
            <button class="tab-btn" onclick="switchTab('books')">📚 Books</button>
        </div>

        <!-- Tab 1: Dashboard -->
        <div id="dashboard" class="tab-content" style="display: none;">
            <h2 style="margin-bottom: var(--space-16);">📊 Your Progress</h2>
            <div class="card-grid" id="dashboardGrid"></div>
            
            <div class="ad-banner-side">
                🎯 Premium Study Guides Available!
            </div>
        </div>

        <!-- Tab 2: AI Planner -->
        <div id="planner" class="tab-content" style="display: none;">
            <h2 style="margin-bottom: var(--space-16);">📅 AI-Powered Study Planner</h2>
            
            <div style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); color: white; padding: var(--space-16); border-radius: var(--radius-base); margin-bottom: var(--space-16);">
                <p>🤖 AI आपके लिए personalized study plan बनाएगा!</p>
            </div>

            <div class="form-group">
                <label>Subject:</label>
                <select id="plannerSubject">
                    <option>Select Subject</option>
                </select>
            </div>

            <div class="form-group">
                <label>Chapter/Topic:</label>
                <input type="text" id="plannerTopic" placeholder="जैसे: Photosynthesis, Laws of Motion">
            </div>

            <div class="form-group">
                <label>Daily Study Time Available (hours):</label>
                <input type="number" id="plannerDuration" min="0.5" max="6" step="0.5" value="2">
            </div>

            <div class="form-group">
                <label>Exam Date:</label>
                <input type="date" id="examDate">
            </div>

            <button class="btn btn-primary" onclick="generateAIPlan()">🤖 Generate AI Plan</button>
            
            <div id="plannerList" style="margin-top: var(--space-20);"></div>
        </div>

        <!-- Tab 3: AI Notes Generator -->
        <div id="notes" class="tab-content" style="display: none;">
            <h2 style="margin-bottom: var(--space-16);">📝 AI NCERT Notes Generator</h2>
            
            <div style="background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%); color: white; padding: var(--space-16); border-radius: var(--radius-base); margin-bottom: var(--space-16);">
                <p>🤖 NCERT से Hindi में Long & Short Notes बनाएं!</p>
            </div>

            <div class="form-group">
                <label>Subject:</label>
                <select id="noteSubject">
                    <option>Select Subject</option>
                </select>
            </div>

            <div class="form-group">
                <label>Chapter Name:</label>
                <input type="text" id="noteTitle" placeholder="जैसे: Chapter 5 - Respiration">
            </div>

            <div class="form-group">
                <label>Note Type:</label>
                <select id="noteType">
                    <option value="short">Short Notes (5 मिनट में पढ़ो)</option>
                    <option value="long">Long Notes (विस्तार से समझो)</option>
                    <option value="both">Both (Short + Long)</option>
                </select>
            </div>

            <button class="btn btn-primary" onclick="generateAINotes()">🤖 Generate Notes</button>
            
            <div id="notesList" style="margin-top: var(--space-20);"></div>
        </div>

        <!-- Tab 4: Resources & Motivation -->
        <div id="motivation" class="tab-content" style="display: none;">
            <h2 style="margin-bottom: var(--space-16);">📚 RBSE Resources & Motivation</h2>
            
            <div style="background: linear-gradient(135deg, var(--color-secondary) 0%, #7c3aed 100%); color: white; padding: var(--space-20); border-radius: var(--radius-base); text-align: center; margin-bottom: var(--space-20);">
                <h3 style="margin-bottom: var(--space-12);">📖 Quote of the Day</h3>
                <p id="motivationQuote" style="font-size: 16px; font-style: italic;">Study smart, not hard! 🔱</p>
            </div>

            <h3 style="margin-bottom: var(--space-16);">🔗 Official RBSE Resources</h3>
            <div class="card-grid">
                <a href="https://rajeduboard.rajasthan.gov.in/" target="_blank" style="text-decoration: none;">
                    <div class="card" style="cursor: pointer; text-align: center;">
                        <h3>📖 RBSE Official Website</h3>
                        <p style="color: var(--color-text-secondary); font-size: 13px;">Syllabus, Exam Updates, Results</p>
                    </div>
                </a>
                
                <a href="https://rajeduboard.rajasthan.gov.in/examschedule.html" target="_blank" style="text-decoration: none;">
                    <div class="card" style="cursor: pointer; text-align: center;">
                        <h3>📅 Exam Schedule</h3>
                        <p style="color: var(--color-text-secondary); font-size: 13px;">Important Dates & Time</p>
                    </div>
                </a>

                <a href="https://rajeduboard.rajasthan.gov.in/syllabusclass10.html" target="_blank" style="text-decoration: none;">
                    <div class="card" style="cursor: pointer; text-align: center;">
                        <h3>📚 Class 10 Syllabus</h3>
                        <p style="color: var(--color-text-secondary); font-size: 13px;">Complete Syllabus PDF</p>
                    </div>
                </a>

                <a href="https://rajeduboard.rajasthan.gov.in/syllabusclass12.html" target="_blank" style="text-decoration: none;">
                    <div class="card" style="cursor: pointer; text-align: center;">
                        <h3>📚 Class 12 Syllabus</h3>
                        <p style="color: var(--color-text-secondary); font-size: 13px;">All Streams Syllabus</p>
                    </div>
                </a>

                <a href="https://textbooks.rajasthan.gov.in/" target="_blank" style="text-decoration: none;">
                    <div class="card" style="cursor: pointer; text-align: center;">
                        <h3>📖 RBSE TextBooks</h3>
                        <p style="color: var(--color-text-secondary); font-size: 13px;">Official Books Download</p>
                    </div>
                </a>

                <a href="https://rajeduboard.rajasthan.gov.in/pastpaper.html" target="_blank" style="text-decoration: none;">
                    <div class="card" style="cursor: pointer; text-align: center;">
                        <h3>📋 Previous Papers</h3>
                        <p style="color: var(--color-text-secondary); font-size: 13px;">Practice Papers & Solutions</p>
                    </div>
                </a>
            </div>

            <h3 style="margin-bottom: var(--space-16); margin-top: var(--space-24);">📚 RBSE Official TextBooks & Materials</h3>
            <div class="card-grid">
                <a href="https://rajeduboard.rajasthan.gov.in/files/book/class10science.pdf" target="_blank" style="text-decoration: none;">
                    <div class="card" style="cursor: pointer; text-align: center;">
                        <h3>🔬 Class 10 Science</h3>
                        <p style="color: var(--color-text-secondary); font-size: 13px;">Official Textbook PDF</p>
                    </div>
                </a>

                <a href="https://rajeduboard.rajasthan.gov.in/files/book/class10mathematics.pdf" target="_blank" style="text-decoration: none;">
                    <div class="card" style="cursor: pointer; text-align: center;">
                        <h3>🔢 Class 10 Mathematics</h3>
                        <p style="color: var(--color-text-secondary); font-size: 13px;">Official Textbook PDF</p>
                    </div>
                </a>

                <a href="https://rajeduboard.rajasthan.gov.in/files/book/class10socialstudies.pdf" target="_blank" style="text-decoration: none;">
                    <div class="card" style="cursor: pointer; text-align: center;">
                        <h3>🌍 Class 10 Social Studies</h3>
                        <p style="color: var(--color-text-secondary); font-size: 13px;">Official Textbook PDF</p>
                    </div>
                </a>

                <a href="https://rajeduboard.rajasthan.gov.in/files/book/class12physics.pdf" target="_blank" style="text-decoration: none;">
                    <div class="card" style="cursor: pointer; text-align: center;">
                        <h3>⚡ Class 12 Physics</h3>
                        <p style="color: var(--color-text-secondary); font-size: 13px;">Official Textbook PDF</p>
                    </div>
                </a>

                <a href="https://rajeduboard.rajasthan.gov.in/files/book/class12chemistry.pdf" target="_blank" style="text-decoration: none;">
                    <div class="card" style="cursor: pointer; text-align: center;">
                        <h3>⚗️ Class 12 Chemistry</h3>
                        <p style="color: var(--color-text-secondary); font-size: 13px;">Official Textbook PDF</p>
                    </div>
                </a>

                <a href="https://rajeduboard.rajasthan.gov.in/files/book/class12biology.pdf" target="_blank" style="text-decoration: none;">
                    <div class="card" style="cursor: pointer; text-align: center;">
                        <h3>🧬 Class 12 Biology</h3>
                        <p style="color: var(--color-text-secondary); font-size: 13px;">Official Textbook PDF</p>
                    </div>
                </a>

                <a href="https://rajeduboard.rajasthan.gov.in/files/book/class12mathematics.pdf" target="_blank" style="text-decoration: none;">
                    <div class="card" style="cursor: pointer; text-align: center;">
                        <h3>🔢 Class 12 Mathematics</h3>
                        <p style="color: var(--color-text-secondary); font-size: 13px;">Official Textbook PDF</p>
                    </div>
                </a>

                <a href="https://rajeduboard.rajasthan.gov.in/files/book/class12accountancy.pdf" target="_blank" style="text-decoration: none;">
                    <div class="card" style="cursor: pointer; text-align: center;">
                        <h3>📊 Class 12 Accountancy</h3>
                        <p style="color: var(--color-text-secondary); font-size: 13px;">Official Textbook PDF</p>
                    </div>
                </a>
            </div>

            <div class="ad-banner-side" style="margin-top: var(--space-20);">
                🎓 Transform Your Study Mindset!
            </div>
        </div>

        <!-- Tab 5: NCERT Books & Solutions (SelfStudys Style) -->
        <div id="books" class="tab-content" style="display: none;">
            <h2 style="margin-bottom: var(--space-16);">📚 NCERT Books, Solutions & Notes</h2>
            
            <div style="background: linear-gradient(135deg, #22c55e 0%, #16a34a 100%); color: white; padding: var(--space-20); border-radius: var(--radius-base); text-align: center; margin-bottom: var(--space-20);">
                <h3 style="margin-bottom: var(--space-12);">📖 Complete Study Resources</h3>
                <p style="font-size: 14px;">NCERT Books, Solutions, Notes - सब कुछ एक जगह!</p>
            </div>

            <h3 style="margin-bottom: var(--space-16);">📚 NCERT Books & Solutions</h3>
            <div class="card-grid">
                <a href="https://www.selfstudys.com/ncert-books" target="_blank" style="text-decoration: none;">
                    <div class="card" style="cursor: pointer; text-align: center;">
                        <h3>📖 NCERT Books (All Classes)</h3>
                        <p style="color: var(--color-text-secondary); font-size: 13px;">Class 6-12 की सभी किताबें</p>
                    </div>
                </a>

                <a href="https://www.selfstudys.com/ncert-solutions" target="_blank" style="text-decoration: none;">
                    <div class="card" style="cursor: pointer; text-align: center;">
                        <h3>✅ NCERT Solutions</h3>
                        <p style="color: var(--color-text-secondary); font-size: 13px;">सभी subjects के detailed solutions</p>
                    </div>
                </a>

                <a href="https://www.selfstudys.com/ncert-notes" target="_blank" style="text-decoration: none;">
                    <div class="card" style="cursor: pointer; text-align: center;">
                        <h3>📝 NCERT Notes</h3>
                        <p style="color: var(--color-text-secondary); font-size: 13px;">Summary और quick revision notes</p>
                    </div>
                </a>

                <a href="https://www.selfstudys.com/exemplar-solutions" target="_blank" style="text-decoration: none;">
                    <div class="card" style="cursor: pointer; text-align: center;">
                        <h3>🎯 Exemplar Solutions</h3>
                        <p style="color: var(--color-text-secondary); font-size: 13px;">Advanced practice problems</p>
                    </div>
                </a>
            </div>

            <h3 style="margin-bottom: var(--space-16); margin-top: var(--space-24);">🔍 Subject-Wise Resources</h3>
            <div class="card-grid">
                <a href="https://www.selfstudys.com/ncert-solutions/class-10-science" target="_blank" style="text-decoration: none;">
                    <div class="card" style="cursor: pointer; text-align: center;">
                        <h3>🔬 Class 10 Science</h3>
                        <p style="color: var(--color-text-secondary); font-size: 13px;">Books + Solutions + Notes</p>
                    </div>
                </a>

                <a href="https://www.selfstudys.com/ncert-solutions/class-12-physics" target="_blank" style="text-decoration: none;">
                    <div class="card" style="cursor: pointer; text-align: center;">
                        <h3>⚡ Class 12 Physics</h3>
                        <p style="color: var(--color-text-secondary); font-size: 13px;">Complete study materials</p>
                    </div>
                </a>

                <a href="https://www.selfstudys.com/ncert-solutions/class-12-chemistry" target="_blank" style="text-decoration: none;">
                    <div class="card" style="cursor: pointer; text-align: center;">
                        <h3>⚗️ Class 12 Chemistry</h3>
                        <p style="color: var(--color-text-secondary); font-size: 13px;">Complete study materials</p>
                    </div>
                </a>

                <a href="https://www.selfstudys.com/ncert-solutions/class-12-biology" target="_blank" style="text-decoration: none;">
                    <div class="card" style="cursor: pointer; text-align: center;">
                        <h3>🧬 Class 12 Biology</h3>
                        <p style="color: var(--color-text-secondary); font-size: 13px;">Complete study materials</p>
                    </div>
                </a>

                <a href="https://www.selfstudys.com/ncert-solutions/class-12-maths" target="_blank" style="text-decoration: none;">
                    <div class="card" style="cursor: pointer; text-align: center;">
                        <h3>🔢 Class 12 Mathematics</h3>
                        <p style="color: var(--color-text-secondary); font-size: 13px;">Complete study materials</p>
                    </div>
                </a>

                <a href="https://www.selfstudys.com/state-board-books" target="_blank" style="text-decoration: none;">
                    <div class="card" style="cursor: pointer; text-align: center;">
                        <h3>🏛️ State Board Books</h3>
                        <p style="color: var(--color-text-secondary); font-size: 13px;">RBSE + अन्य boards</p>
                    </div>
                </a>
            </div>

            <h3 style="margin-bottom: var(--space-16); margin-top: var(--space-24);">🎯 Exam-Specific Resources</h3>
            <div class="card-grid">
                <a href="https://www.selfstudys.com/neet-solutions" target="_blank" style="text-decoration: none;">
                    <div class="card" style="cursor: pointer; text-align: center;">
                        <h3>🏥 NEET Preparation</h3>
                        <p style="color: var(--color-text-secondary); font-size: 13px;">Complete NEET study guide</p>
                    </div>
                </a>

                <a href="https://www.selfstudys.com/jee-solutions" target="_blank" style="text-decoration: none;">
                    <div class="card" style="cursor: pointer; text-align: center;">
                        <h3>🔬 JEE Preparation</h3>
                        <p style="color: var(--color-text-secondary); font-size: 13px;">Complete JEE study guide</p>
                    </div>
                </a>

                <a href="https://www.selfstudys.com/cbse-board-exam-solutions" target="_blank" style="text-decoration: none;">
                    <div class="card" style="cursor: pointer; text-align: center;">
                        <h3>📋 CBSE Board Exam</h3>
                        <p style="color: var(--color-text-secondary); font-size: 13px;">Board exam preparation</p>
                    </div>
                </a>

                <a href="https://www.selfstudys.com/previous-year-papers" target="_blank" style="text-decoration: none;">
                    <div class="card" style="cursor: pointer; text-align: center;">
                        <h3>📄 Previous Year Papers</h3>
                        <p style="color: var(--color-text-secondary); font-size: 13px;">Solved past papers</p>
                    </div>
                </a>
            </div>

            <div class="ad-banner-side" style="margin-top: var(--space-20);">
                📚 सभी Resources Free Download के लिए उपलब्ध!
            </div>
        </div>
    </div>

    <script>
        let appData = {
            selectedClass: '12th',
            selectedStream: 'PCB',
            setupComplete: false,
            streamsData: {
                'PCB': ['Physics', 'Chemistry', 'Biology'],
                'PCA': ['Physics', 'Chemistry', 'Accountancy'],
                'PCM': ['Physics', 'Chemistry', 'Mathematics'],
                'Commerce': ['Accounts', 'Economics', 'Business Studies'],
                'Arts': ['History', 'Geography', 'Political Science'],
                '10th': ['Science', 'Social Studies', 'Mathematics', 'English']
            },
            planner: [],
            notes: [],
            subjects: ['Physics', 'Chemistry', 'Biology']
        };

        function selectClass(classVal) {
            appData.selectedClass = classVal;
            document.querySelectorAll('.setup-option').forEach((el, idx) => {
                if (idx < 2) el.classList.toggle('selected');
            });
            
            if (classVal === '10th') {
                document.getElementById('streamOptions').style.display = 'none';
                appData.selectedStream = null;
            } else {
                document.getElementById('streamOptions').style.display = 'block';
            }
        }

        function selectStream(stream) {
            appData.selectedStream = stream;
            document.querySelectorAll('.setup-options')[1].querySelectorAll('.setup-option').forEach(el => {
                el.classList.remove('selected');
            });
            event.target.classList.add('selected');
        }

        function completeSetup() {
            appData.setupComplete = true;
            appData.subjects = appData.streamsData[appData.selectedStream || appData.selectedClass];
            
            document.getElementById('setupSection').style.display = 'none';
            document.getElementById('mainTabs').style.display = 'flex';
            document.getElementById('dashboard').style.display = 'block';
            
            updateSubjectSelects();
            renderDashboard();
        }

        function updateSubjectSelects() {
            const subjects = appData.subjects;
            const plannerSubject = document.getElementById('plannerSubject');
            const noteSubject = document.getElementById('noteSubject');
            
            plannerSubject.innerHTML = '<option>Select Subject</option>' + subjects.map(s => `<option>${s}</option>`).join('');
            noteSubject.innerHTML = '<option>Select Subject</option>' + subjects.map(s => `<option>${s}</option>`).join('');
        }

        function switchTab(tabName) {
            document.querySelectorAll('.tab-content').forEach(el => el.style.display = 'none');
            document.querySelectorAll('.tab-btn').forEach(el => el.classList.remove('active'));
            
            document.getElementById(tabName).style.display = 'block';
            event.target.classList.add('active');
        }

        function renderDashboard() {
            const grid = document.getElementById('dashboardGrid');
            grid.innerHTML = appData.subjects.map(subject => `
                <div class="card">
                    <h3>${subject}</h3>
                    <div style="font-size: 13px; color: var(--color-text-secondary); margin-bottom: var(--space-12);">
                        0/5 Topics
                    </div>
                    <div class="progress-bar">
                        <div class="progress-fill" style="width: 0%"></div>
                    </div>
                </div>
            `).join('');
        }

        function generateAIPlan() {
            const subject = document.getElementById('plannerSubject').value;
            const topic = document.getElementById('plannerTopic').value;
            const dailyHours = document.getElementById('plannerDuration').value;
            const examDate = document.getElementById('examDate').value;

            if (!topic || !examDate) {
                alert('कृपया सभी fields fill करो');
                return;
            }

            const aiPlan = `
🤖 AI GENERATED PLAN

📚 Subject: ${subject}
📖 Topic: ${topic}
⏱️ Daily Time: ${dailyHours} hours
📅 Exam Date: ${new Date(examDate).toLocaleDateString('hi-IN')}

✅ RECOMMENDED STUDY SCHEDULE:
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Day 1-2: Theory को समझो (Video देखो)
Day 3-4: Important Points को notes बनाओ
Day 5: Previous Year Questions solve करो
Day 6: Mock Test दो
Day 7: Revision करो

📊 Study Breakdown:
• Reading: 40%
• Writing Notes: 30%
• Practice Questions: 20%
• Revision: 10%

💡 Tips:
✓ Early morning study करो (5 AM)
✓ 45 min study + 5 min break
✓ Mobile दूर रखो
✓ Daily revision करो
            `;

            appData.planner.push({ 
                subject, 
                topic, 
                duration: dailyHours,
                examDate,
                aiGenerated: true,
                plan: aiPlan 
            });
            
            document.getElementById('plannerTopic').value = '';
            document.getElementById('examDate').value = '';
            renderPlannerList();
        }

        function renderPlannerList() {
            const list = document.getElementById('plannerList');
            list.innerHTML = appData.planner.map((item, idx) => `
                <div class="item-card">
                    <h4>🤖 ${item.topic}</h4>
                    <div class="meta">📚 ${item.subject} | ⏱️ ${item.duration} hours | 📅 ${item.examDate || 'N/A'}</div>
                    ${item.aiGenerated ? `<div style="background: var(--color-bg); padding: var(--space-12); border-radius: var(--radius-base); margin-bottom: var(--space-12); white-space: pre-wrap; font-size: 12px;">${item.plan}</div>` : ''}
                    <button class="btn btn-secondary" onclick="removePlannerItem(${idx})" style="font-size: 12px; padding: 6px 12px;">Delete</button>
                </div>
            `).join('');
        }

        function removePlannerItem(idx) {
            appData.planner.splice(idx, 1);
            renderPlannerList();
        }

        function generateAINotes() {
            const subject = document.getElementById('noteSubject').value;
            const chapter = document.getElementById('noteTitle').value;
            const noteType = document.getElementById('noteType').value;

            if (!chapter) {
                alert('कृपया Chapter का नाम दर्ज करो');
                return;
            }

            const shortNotes = `
📝 SHORT NOTES (5 मिनट में पढ़ो)
━━━━━━━━━━━━━━━━━━━━━━━━━━━

🔑 Key Points:
• Definition: सरल भाषा में परिभाषा
• Formula/Law: महत्वपूर्ण formula
• Example: 1-2 उदाहरण
• Application: कहाँ use होता है

⭐ याद रखो:
✓ Main concept क्या है
✓ क्यों महत्वपूर्ण है
✓ Real-life example

📊 Quick Facts:
→ Important dates/names
→ Special characteristics
→ Common mistakes
            `;

            const longNotes = `
📖 DETAILED NOTES (विस्तार से समझो)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

1️⃣ INTRODUCTION
• Historical background
• Discovery/Development
• Why this topic matters

2️⃣ DETAILED EXPLANATION
• Complete definition
• Step-by-step process
• Related concepts
• Interconnections

3️⃣ FORMULAS & LAWS
• All important formulas
• When to use them
• Derivations
• Units & measurements

4️⃣ EXAMPLES & APPLICATIONS
• Solved problems
• Real-world applications
• Case studies

5️⃣ IMPORTANT QUESTIONS
• What? (Definition)
• Why? (Importance)
• How? (Process)
• Where? (Application)

6️⃣ COMMON MISTAKES
• लोग क्या गलत समझते हैं
• सही approach क्या है

7️⃣ SUMMARY
• एक नज़र में सब कुछ
• याद रखने वाली बातें
            `;

            let content = '';
            if (noteType === 'short') content = shortNotes;
            else if (noteType === 'long') content = longNotes;
            else content = shortNotes + '\n\n' + longNotes;

            appData.notes.push({ 
                subject, 
                title: chapter, 
                content,
                aiGenerated: true,
                type: noteType
            });
            
            document.getElementById('noteTitle').value = '';
            renderNotesList();
        }

        function renderNotesList() {
            const list = document.getElementById('notesList');
            list.innerHTML = appData.notes.map((note, idx) => `
                <div class="item-card">
                    <h4>${note.aiGenerated ? '🤖' : '📝'} ${note.title}</h4>
                    <div class="meta">📚 ${note.subject} ${note.type ? `| Type: ${note.type === 'short' ? 'Short Notes' : note.type === 'long' ? 'Long Notes' : 'Both'}` : ''}</div>
                    <div style="background: var(--color-bg); padding: var(--space-12); border-radius: var(--radius-base); margin-bottom: var(--space-12); white-space: pre-wrap; font-size: 13px; max-height: 400px; overflow-y: auto;">
                        ${note.content}
                    </div>
                    <button class="btn btn-secondary" onclick="removeNote(${idx})" style="font-size: 12px; padding: 6px 12px;">Delete</button>
                </div>
            `).join('');
        }

        function removeNote(idx) {
            appData.notes.splice(idx, 1);
            renderNotesList();
        }
    </script>
