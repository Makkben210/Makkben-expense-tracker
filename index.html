<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>💰 MAKKBEN Smart Expense Tracker</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/xlsx/dist/xlsx.full.min.js"></script>
    <style>
        :root {
            --primary: #D4AF37; /* Gold */
            --primary-dark: #B8860B;
            --secondary: #FFD700;
            --danger: #C41E3A;
            --warning: #FFA500;
            --success: #32CD32;
            --background: #0A0A0A;
            --surface: #1A1A1A;
            --text: #F5F5F5;
            --text-light: #AAAAAA;
            --border: #333333;
            --shadow: 0 4px 20px rgba(212, 175, 55, 0.15);
            --radius: 12px;
            --gold-gradient: linear-gradient(135deg, #D4AF37, #FFD700, #B8860B);
            --dark-gradient: linear-gradient(135deg, #1A1A1A, #0A0A0A);
            --malek-color: #3498db;
            --sabrina-color: #e74c3c;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, sans-serif;
            -webkit-tap-highlight-color: transparent;
        }

        html {
            font-size: 14px;
            overflow-x: hidden;
            background: var(--background);
        }

        body {
            background: var(--background);
            color: var(--text);
            max-width: 100%;
            min-height: 100vh;
            padding: 15px;
            padding-bottom: 180px;
            position: relative;
        }

        /* Profile Selector */
        .profile-selector {
            display: flex;
            gap: 10px;
            margin-bottom: 15px;
        }

        .profile-btn {
            flex: 1;
            padding: 12px;
            border: 2px solid var(--border);
            border-radius: var(--radius);
            background: var(--surface);
            color: var(--text);
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 8px;
        }

        .profile-btn.active {
            border-color: var(--primary);
            background: linear-gradient(135deg, rgba(212, 175, 55, 0.1), rgba(26, 26, 26, 0.8));
        }

        .profile-btn.malek.active {
            border-color: var(--malek-color);
            background: linear-gradient(135deg, rgba(52, 152, 219, 0.1), rgba(26, 26, 26, 0.8));
        }

        .profile-btn.sabrina.active {
            border-color: var(--sabrina-color);
            background: linear-gradient(135deg, rgba(231, 76, 60, 0.1), rgba(26, 26, 26, 0.8));
        }

        /* Header */
        .app-header {
            background: linear-gradient(135deg, #1A1A1A, #2A2A2A);
            border-radius: var(--radius);
            padding: 20px;
            margin-bottom: 20px;
            color: var(--primary);
            position: relative;
            overflow: hidden;
            border: 1px solid rgba(212, 175, 55, 0.3);
            box-shadow: var(--shadow);
        }

        .app-header::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: var(--gold-gradient);
        }

        .app-header h1 {
            font-size: 22px;
            font-weight: 700;
            margin-bottom: 5px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .user-info {
            display: flex;
            align-items: center;
            gap: 10px;
            margin-top: 10px;
        }

        .user-avatar {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            color: white;
            font-size: 18px;
        }

        .avatar-malek {
            background: linear-gradient(135deg, var(--malek-color), #2980b9);
        }

        .avatar-sabrina {
            background: linear-gradient(135deg, var(--sabrina-color), #c0392b);
        }

        .signature {
            position: absolute;
            right: 20px;
            bottom: 10px;
            font-size: 12px;
            opacity: 0.8;
            color: var(--primary);
        }

        .quick-stats {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 10px;
            margin: 20px 0;
        }

        .stat-card {
            background: var(--surface);
            border-radius: var(--radius);
            padding: 15px;
            text-align: center;
            box-shadow: var(--shadow);
            min-height: 80px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            border: 1px solid var(--border);
            transition: transform 0.2s ease, border-color 0.2s ease;
        }

        .stat-card:hover {
            transform: translateY(-2px);
            border-color: var(--primary);
        }

        .stat-value {
            font-size: 18px;
            font-weight: 700;
            margin-bottom: 5px;
            white-space: nowrap;
            overflow: hidden;
            text-overflow: ellipsis;
            color: var(--primary);
        }

        .stat-label {
            font-size: 11px;
            color: var(--text-light);
        }

        .budget-warning {
            color: var(--danger) !important;
            font-weight: bold;
        }

        .budget-close {
            color: var(--warning) !important;
            font-weight: bold;
        }

        /* Navigation */
        .nav-tabs {
            display: flex;
            background: var(--surface);
            border-radius: var(--radius);
            padding: 5px;
            margin-bottom: 20px;
            overflow-x: auto;
            -webkit-overflow-scrolling: touch;
            scrollbar-width: none;
            border: 1px solid var(--border);
        }

        .nav-tabs::-webkit-scrollbar {
            display: none;
        }

        .nav-tab {
            flex: 1;
            min-width: 70px;
            padding: 12px 10px;
            border: none;
            background: transparent;
            border-radius: 8px;
            font-size: 12px;
            font-weight: 600;
            cursor: pointer;
            white-space: nowrap;
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 5px;
            color: var(--text-light);
            transition: all 0.3s ease;
        }

        .nav-tab.active {
            background: linear-gradient(135deg, #D4AF37, #B8860B);
            color: #000;
            box-shadow: 0 2px 10px rgba(212, 175, 55, 0.3);
        }

        .tab-icon {
            font-size: 16px;
        }

        /* Content Area */
        .content-area {
            min-height: 300px;
            position: relative;
        }

        .tab-content {
            display: none;
            animation: fadeIn 0.3s ease;
        }

        .tab-content.active {
            display: block;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        /* Quick Add */
        .quick-add-section {
            position: fixed;
            bottom: 20px;
            left: 15px;
            right: 15px;
            background: var(--surface);
            border-radius: var(--radius);
            padding: 15px;
            box-shadow: 0 -10px 30px rgba(0,0,0,0.5);
            z-index: 1000;
            border: 2px solid var(--primary);
        }

        .quick-inputs {
            display: flex;
            gap: 10px;
            margin-bottom: 15px;
        }

        .amount-input {
            flex: 2;
            padding: 15px;
            border: 2px solid var(--border);
            border-radius: var(--radius);
            font-size: 20px;
            font-weight: 700;
            text-align: center;
            outline: none;
            min-width: 0;
            background: var(--background);
            color: var(--primary);
        }

        .currency-select {
            flex: 1;
            padding: 15px;
            border: 2px solid var(--border);
            border-radius: var(--radius);
            background: var(--background);
            font-size: 14px;
            font-weight: 600;
            min-width: 0;
            color: var(--text);
        }

        .category-select {
            width: 100%;
            padding: 12px;
            border: 2px solid var(--border);
            border-radius: var(--radius);
            background: var(--background);
            font-size: 14px;
            margin-bottom: 10px;
            color: var(--text);
        }

        .profile-select {
            width: 100%;
            padding: 12px;
            border: 2px solid var(--border);
            border-radius: var(--radius);
            background: var(--background);
            font-size: 14px;
            margin-bottom: 10px;
            color: var(--text);
        }

        .quick-actions {
            display: flex;
            gap: 10px;
        }

        .quick-btn {
            flex: 1;
            padding: 12px;
            border: none;
            border-radius: var(--radius);
            font-size: 14px;
            font-weight: 600;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 8px;
            transition: transform 0.2s ease;
        }

        .quick-btn:active {
            transform: scale(0.98);
        }

        .save-btn {
            background: linear-gradient(135deg, #D4AF37, #B8860B);
            color: #000;
        }

        .add-btn {
            background: linear-gradient(135deg, #333333, #1A1A1A);
            color: var(--primary);
            border: 1px solid var(--primary);
        }

        /* Cards */
        .card {
            background: var(--surface);
            border-radius: var(--radius);
            padding: 20px;
            margin-bottom: 15px;
            box-shadow: var(--shadow);
            border: 1px solid var(--border);
        }

        .card-title {
            font-size: 16px;
            font-weight: 600;
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            color: var(--primary);
        }

        /* Budget Cards */
        .budget-card {
            border-left: 5px solid;
            margin-bottom: 10px;
            padding: 15px;
            background: rgba(26, 26, 26, 0.8);
            border-radius: var(--radius);
        }

        .budget-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 10px;
        }

        .budget-name {
            font-weight: 600;
            font-size: 14px;
            color: var(--text);
        }

        .budget-amount {
            font-weight: 700;
            font-size: 14px;
        }

        .budget-progress {
            height: 8px;
            background: var(--border);
            border-radius: 4px;
            overflow: hidden;
            margin: 10px 0;
        }

        .budget-progress-bar {
            height: 100%;
            background: linear-gradient(90deg, #D4AF37, #FFD700);
            border-radius: 4px;
            transition: width 0.3s ease;
        }

        .budget-stats {
            display: flex;
            justify-content: space-between;
            font-size: 11px;
            color: var(--text-light);
        }

        /* Expense List */
        .expense-item {
            display: flex;
            align-items: center;
            padding: 15px;
            border-bottom: 1px solid var(--border);
            position: relative;
            transition: background-color 0.2s ease;
        }

        .expense-item:hover {
            background: rgba(212, 175, 55, 0.05);
        }

        .expense-item:last-child {
            border-bottom: none;
        }

        .expense-icon {
            width: 40px;
            height: 40px;
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 18px;
            color: #000;
            margin-right: 12px;
            flex-shrink: 0;
            background: linear-gradient(135deg, #D4AF37, #FFD700);
        }

        .expense-details {
            flex: 1;
            min-width: 0;
        }

        .expense-title {
            font-weight: 600;
            margin-bottom: 4px;
            white-space: nowrap;
            overflow: hidden;
            text-overflow: ellipsis;
            font-size: 14px;
        }

        .expense-meta {
            font-size: 11px;
            color: var(--text-light);
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .expense-amount {
            text-align: right;
            flex-shrink: 0;
            margin-left: 10px;
        }

        .amount-primary {
            font-size: 16px;
            font-weight: 700;
            white-space: nowrap;
            color: var(--primary);
        }

        .amount-secondary {
            font-size: 10px;
            color: var(--text-light);
            white-space: nowrap;
        }

        /* User badge in expenses */
        .user-badge {
            padding: 2px 8px;
            border-radius: 10px;
            font-size: 10px;
            font-weight: 600;
            color: white;
        }

        .user-badge.malek {
            background: linear-gradient(135deg, var(--malek-color), #2980b9);
        }

        .user-badge.sabrina {
            background: linear-gradient(135deg, var(--sabrina-color), #c0392b);
        }

        /* To-Buy List */
        .todo-item {
            display: flex;
            align-items: center;
            padding: 15px;
            border-bottom: 1px solid var(--border);
            transition: background-color 0.2s ease;
        }

        .todo-item:hover {
            background: rgba(212, 175, 55, 0.05);
        }

        .todo-checkbox {
            margin-right: 12px;
            width: 20px;
            height: 20px;
            accent-color: var(--primary);
        }

        .todo-content {
            flex: 1;
            min-width: 0;
        }

        .todo-actions {
            display: flex;
            gap: 8px;
        }

        /* Form Elements */
        .form-group {
            margin-bottom: 15px;
        }

        .form-label {
            display: block;
            margin-bottom: 5px;
            font-weight: 600;
            font-size: 13px;
            color: var(--text-light);
        }

        .form-input {
            width: 100%;
            padding: 12px;
            border: 2px solid var(--border);
            border-radius: var(--radius);
            font-size: 14px;
            background: var(--background);
            color: var(--text);
            transition: border-color 0.3s ease;
        }

        .form-input:focus {
            border-color: var(--primary);
            outline: none;
        }

        .btn {
            padding: 12px 20px;
            border: none;
            border-radius: var(--radius);
            font-size: 14px;
            font-weight: 600;
            cursor: pointer;
            display: inline-flex;
            align-items: center;
            justify-content: center;
            gap: 8px;
            transition: all 0.3s ease;
        }

        .btn:hover {
            transform: translateY(-2px);
        }

        .btn-primary {
            background: linear-gradient(135deg, #D4AF37, #B8860B);
            color: #000;
            border: 1px solid rgba(212, 175, 55, 0.5);
        }

        .btn-secondary {
            background: linear-gradient(135deg, #333, #222);
            color: var(--primary);
            border: 1px solid var(--primary);
        }

        .btn-danger {
            background: linear-gradient(135deg, #C41E3A, #A8152F);
            color: white;
        }

        /* Modal */
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0,0,0,0.8);
            z-index: 2000;
            align-items: center;
            justify-content: center;
            padding: 20px;
            backdrop-filter: blur(5px);
        }

        .modal.active {
            display: flex;
            animation: modalFadeIn 0.3s ease;
        }

        @keyframes modalFadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        .modal-content {
            background: var(--surface);
            border-radius: var(--radius);
            padding: 20px;
            width: 100%;
            max-width: 500px;
            max-height: 80vh;
            overflow-y: auto;
            -webkit-overflow-scrolling: touch;
            border: 2px solid var(--primary);
            box-shadow: 0 20px 60px rgba(0,0,0,0.5);
        }

        .modal-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
            padding-bottom: 15px;
            border-bottom: 2px solid var(--border);
        }

        .modal-title {
            font-size: 18px;
            font-weight: 700;
            color: var(--primary);
        }

        .close-modal {
            background: none;
            border: none;
            font-size: 24px;
            cursor: pointer;
            color: var(--primary);
            transition: transform 0.2s ease;
        }

        .close-modal:hover {
            transform: scale(1.1);
        }

        /* Utility */
        .text-danger { color: var(--danger); }
        .text-warning { color: var(--warning); }
        .text-success { color: var(--success); }
        .text-muted { color: var(--text-light); font-size: 11px; }
        .text-gold { color: var(--primary); }

        .d-flex { display: flex; }
        .justify-between { justify-content: space-between; }
        .align-center { align-items: center; }
        .gap-10 { gap: 10px; }
        .mb-15 { margin-bottom: 15px; }
        .mt-15 { margin-top: 15px; }
        .w-100 { width: 100%; }
        .flex-1 { flex: 1; }

        /* Scrollable container */
        .scrollable {
            overflow-y: auto;
            -webkit-overflow-scrolling: touch;
            max-height: 400px;
        }

        /* Ensure no text overflow */
        .truncate {
            white-space: nowrap;
            overflow: hidden;
            text-overflow: ellipsis;
        }

        /* Responsive adjustments */
        @media (max-width: 360px) {
            html { font-size: 13px; }
            .stat-value { font-size: 16px; }
            .amount-primary { font-size: 14px; }
        }

        /* Loading */
        .loading {
            text-align: center;
            padding: 40px;
            color: var(--text-light);
        }

        /* Currency converter */
        .converter-box {
            background: var(--surface);
            border-radius: var(--radius);
            padding: 20px;
            margin-bottom: 20px;
            box-shadow: var(--shadow);
            border: 1px solid var(--border);
        }

        .converter-row {
            display: flex;
            align-items: center;
            gap: 10px;
            margin: 15px 0;
        }

        .converter-input {
            flex: 1;
            padding: 15px;
            border: 2px solid var(--border);
            border-radius: var(--radius);
            font-size: 18px;
            font-weight: 600;
            text-align: right;
            min-width: 0;
            background: var(--background);
            color: var(--primary);
        }

        .converter-label {
            min-width: 60px;
            font-weight: 600;
            font-size: 14px;
            color: var(--text-light);
        }

        /* Receipt viewer */
        .receipt-preview {
            width: 100%;
            max-height: 300px;
            object-fit: contain;
            border-radius: var(--radius);
            border: 2px solid var(--border);
            margin-top: 10px;
        }

        /* Calendar view */
        .calendar-container {
            background: var(--surface);
            border-radius: var(--radius);
            padding: 20px;
            box-shadow: var(--shadow);
            border: 1px solid var(--border);
        }

        .calendar-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
            padding-bottom: 15px;
            border-bottom: 2px solid var(--border);
        }

        .calendar-grid {
            display: grid;
            grid-template-columns: repeat(7, 1fr);
            gap: 5px;
            margin-bottom: 20px;
        }

        .calendar-day-header {
            text-align: center;
            padding: 10px;
            font-weight: bold;
            color: var(--primary);
            font-size: 12px;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .calendar-day {
            aspect-ratio: 1;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            border-radius: 8px;
            font-size: 12px;
            background: var(--background);
            border: 2px solid var(--border);
            cursor: pointer;
            transition: all 0.2s ease;
            padding: 5px;
            position: relative;
        }

        .calendar-day:hover {
            border-color: var(--primary);
            transform: scale(1.05);
        }

        .calendar-day.has-expenses {
            background: linear-gradient(135deg, rgba(212, 175, 55, 0.2), rgba(255, 215, 0, 0.1));
            border-color: var(--primary);
            color: var(--primary);
        }

        .calendar-day.today {
            background: linear-gradient(135deg, #D4AF37, #FFD700);
            color: #000;
            border-color: var(--primary);
            font-weight: bold;
        }

        .day-expense-total {
            font-size: 8px;
            margin-top: 2px;
            color: var(--text-light);
        }

        /* Month selector */
        .month-selector {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 20px;
            margin: 20px 0;
        }

        .month-btn {
            background: linear-gradient(135deg, #D4AF37, #B8860B);
            border: none;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            font-size: 18px;
            cursor: pointer;
            color: #000;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: transform 0.2s ease;
        }

        .month-btn:hover {
            transform: scale(1.1);
        }

        .month-display {
            font-size: 18px;
            font-weight: 700;
            min-width: 150px;
            text-align: center;
            color: var(--primary);
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        /* Goals Section */
        .goals-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 15px;
        }

        .goal-card {
            background: linear-gradient(135deg, rgba(212, 175, 55, 0.1), rgba(26, 26, 26, 0.8));
            border: 2px solid var(--primary);
            border-radius: var(--radius);
            padding: 20px;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .goal-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 30px rgba(212, 175, 55, 0.2);
        }

        .goal-header {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            margin-bottom: 15px;
        }

        .goal-title {
            font-size: 18px;
            font-weight: 700;
            color: var(--primary);
            flex: 1;
        }

        .goal-priority {
            padding: 4px 12px;
            border-radius: 20px;
            font-size: 11px;
            font-weight: 600;
            text-transform: uppercase;
        }

        .priority-high { background: rgba(196, 30, 58, 0.2); color: #C41E3A; border: 1px solid rgba(196, 30, 58, 0.3); }
        .priority-medium { background: rgba(255, 165, 0, 0.2); color: #FFA500; border: 1px solid rgba(255, 165, 0, 0.3); }
        .priority-low { background: rgba(50, 205, 50, 0.2); color: #32CD32; border: 1px solid rgba(50, 205, 50, 0.3); }

        .goal-progress {
            margin: 20px 0;
        }

        .progress-bar {
            height: 10px;
            background: var(--border);
            border-radius: 5px;
            overflow: hidden;
            margin-bottom: 8px;
        }

        .progress-fill {
            height: 100%;
            background: linear-gradient(90deg, #D4AF37, #FFD700);
            border-radius: 5px;
            transition: width 0.5s ease;
        }

        .progress-stats {
            display: flex;
            justify-content: space-between;
            font-size: 12px;
            color: var(--text-light);
        }

        .goal-details {
            font-size: 13px;
            color: var(--text-light);
            margin: 15px 0;
            line-height: 1.5;
        }

        .goal-actions {
            display: flex;
            gap: 10px;
            margin-top: 15px;
        }

        /* Badges */
        .badge {
            display: inline-block;
            padding: 4px 8px;
            border-radius: 20px;
            font-size: 10px;
            font-weight: 600;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }

        .badge-low {
            background: rgba(50, 205, 50, 0.2);
            color: #32CD32;
            border: 1px solid rgba(50, 205, 50, 0.3);
        }

        .badge-medium {
            background: rgba(255, 165, 0, 0.2);
            color: #FFA500;
            border: 1px solid rgba(255, 165, 0, 0.3);
        }

        .badge-high {
            background: rgba(212, 175, 55, 0.2);
            color: #D4AF37;
            border: 1px solid rgba(212, 175, 55, 0.3);
        }

        /* Filter Section */
        .filter-section {
            background: var(--surface);
            border-radius: var(--radius);
            padding: 15px;
            margin-bottom: 20px;
            border: 1px solid var(--border);
        }

        .filter-row {
            display: flex;
            gap: 10px;
            margin-bottom: 10px;
            flex-wrap: wrap;
        }

        .filter-select {
            flex: 1;
            min-width: 120px;
            padding: 10px;
            border: 2px solid var(--border);
            border-radius: var(--radius);
            background: var(--background);
            color: var(--text);
            font-size: 12px;
        }

        /* Action buttons */
        .item-actions {
            display: flex;
            gap: 5px;
        }

        .item-actions .btn {
            padding: 6px 10px;
            font-size: 12px;
        }

        /* Profile stats */
        .profile-stats {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 10px;
            margin: 15px 0;
        }

        .profile-stat-card {
            background: var(--surface);
            border-radius: var(--radius);
            padding: 15px;
            text-align: center;
            border: 1px solid var(--border);
        }

        .profile-stat-card.malek {
            border-color: var(--malek-color);
        }

        .profile-stat-card.sabrina {
            border-color: var(--sabrina-color);
        }
    </style>
</head>
<body>
    <!-- Profile Selector -->
    <div class="profile-selector">
        <button class="profile-btn malek active" onclick="switchProfile('malek')">
            <i class="fas fa-user"></i> Malek
        </button>
        <button class="profile-btn sabrina" onclick="switchProfile('sabrina')">
            <i class="fas fa-user"></i> Sabrina
        </button>
    </div>

    <!-- App Header -->
    <div class="app-header">
        <h1><i class="fas fa-crown"></i> MAKKBEN Smart Tracker</h1>
        <div class="signature">Shared: Malek & Sabrina</div>
        
        <div class="user-info">
            <div class="user-avatar avatar-malek" id="currentAvatar">M</div>
            <div>
                <div id="currentUserName">Malek</div>
                <div class="text-muted" id="currentUserEmail">Personal Expense Tracker</div>
            </div>
        </div>
        
        <!-- Quick Stats -->
        <div class="quick-stats">
            <div class="stat-card">
                <div class="stat-value" id="totalBalance">0 AED</div>
                <div class="stat-label">Total Balance</div>
            </div>
            <div class="stat-card">
                <div class="stat-value" id="monthExpenses">0 AED</div>
                <div class="stat-label">This Month</div>
            </div>
            <div class="stat-card">
                <div class="stat-value" id="remainingBalance">0 AED</div>
                <div class="stat-label">Remaining</div>
            </div>
        </div>
    </div>

    <!-- Navigation Tabs -->
    <div class="nav-tabs">
        <button class="nav-tab active" onclick="switchTab('dashboard')">
            <i class="fas fa-chart-pie tab-icon"></i>
            <span>Dashboard</span>
        </button>
        <button class="nav-tab" onclick="switchTab('expenses')">
            <i class="fas fa-receipt tab-icon"></i>
            <span>Expenses</span>
        </button>
        <button class="nav-tab" onclick="switchTab('budgets')">
            <i class="fas fa-chart-pie tab-icon"></i>
            <span>Budgets</span>
        </button>
        <button class="nav-tab" onclick="switchTab('calendar')">
            <i class="fas fa-calendar-alt tab-icon"></i>
            <span>Calendar</span>
        </button>
        <button class="nav-tab" onclick="switchTab('todo')">
            <i class="fas fa-list-check tab-icon"></i>
            <span>To-Buy</span>
        </button>
        <button class="nav-tab" onclick="switchTab('goals')">
            <i class="fas fa-bullseye tab-icon"></i>
            <span>Goals</span>
        </button>
        <button class="nav-tab" onclick="switchTab('profiles')">
            <i class="fas fa-users tab-icon"></i>
            <span>Profiles</span>
        </button>
        <button class="nav-tab" onclick="switchTab('settings')">
            <i class="fas fa-cog tab-icon"></i>
            <span>Settings</span>
        </button>
    </div>

    <!-- Main Content Area -->
    <div class="content-area">
        <!-- Dashboard Tab -->
        <div id="dashboard" class="tab-content active">
            <div class="card">
                <div class="card-title">
                    <span>Monthly Overview</span>
                    <span id="currentMonth"></span>
                </div>
                <canvas id="dashboardChart"></canvas>
            </div>
            
            <div class="card">
                <div class="card-title">
                    <span>Recent Expenses</span>
                    <button class="btn btn-secondary btn-sm" onclick="switchTab('expenses')">
                        <i class="fas fa-eye"></i> View All
                    </button>
                </div>
                <div id="recentExpenses" class="scrollable" style="max-height: 250px;"></div>
            </div>
            
            <div class="card">
                <div class="card-title">
                    <span>Profile Spending (This Month)</span>
                </div>
                <div class="profile-stats">
                    <div class="profile-stat-card malek">
                        <div class="stat-label">Malek</div>
                        <div class="stat-value" id="malekMonthSpending">0 AED</div>
                    </div>
                    <div class="profile-stat-card sabrina">
                        <div class="stat-label">Sabrina</div>
                        <div class="stat-value" id="sabrinaMonthSpending">0 AED</div>
                    </div>
                </div>
            </div>
            
            <div class="card">
                <div class="card-title">
                    <span>Quick Actions</span>
                </div>
                <div class="d-flex gap-10">
                    <button class="btn btn-primary flex-1" onclick="showAddReceiptModal()">
                        <i class="fas fa-camera"></i> Add Expense
                    </button>
                    <button class="btn btn-secondary flex-1" onclick="showTodoModal()">
                        <i class="fas fa-list"></i> Add To-Buy
                    </button>
                </div>
            </div>
        </div>

        <!-- Expenses Tab -->
        <div id="expenses" class="tab-content">
            <div class="filter-section">
                <div class="filter-row">
                    <select class="filter-select" id="filterCategory" onchange="filterExpenses()">
                        <option value="">All Categories</option>
                    </select>
                    <select class="filter-select" id="filterMonth" onchange="filterExpenses()">
                        <option value="">All Time</option>
                    </select>
                    <select class="filter-select" id="filterCurrency" onchange="filterExpenses()">
                        <option value="">All Currencies</option>
                        <option value="AED">AED</option>
                        <option value="DZD">DZD</option>
                    </select>
                    <select class="filter-select" id="filterProfile" onchange="filterExpenses()">
                        <option value="">Both Profiles</option>
                        <option value="malek">Malek</option>
                        <option value="sabrina">Sabrina</option>
                    </select>
                </div>
                <div class="d-flex justify-between">
                    <div>
                        <span class="text-muted">Total: </span>
                        <span class="text-gold" id="filteredTotal">0 AED</span>
                    </div>
                    <div>
                        <span class="text-muted">Count: </span>
                        <span class="text-gold" id="filteredCount">0</span>
                    </div>
                </div>
            </div>
            
            <div class="card">
                <div class="card-title">
                    <span>All Expenses</span>
                    <div class="d-flex gap-10">
                        <button class="btn btn-secondary btn-sm" onclick="exportToExcel()">
                            <i class="fas fa-file-excel"></i> Excel
                        </button>
                        <button class="btn btn-danger btn-sm" onclick="exportToPDF()">
                            <i class="fas fa-file-pdf"></i> PDF
                        </button>
                        <button class="btn btn-primary btn-sm" onclick="showAddReceiptModal()">
                            <i class="fas fa-plus"></i> Add
                        </button>
                    </div>
                </div>
                <div id="expensesList" class="scrollable"></div>
            </div>
        </div>

        <!-- Budgets Tab -->
        <div id="budgets" class="tab-content">
            <div class="card">
                <div class="card-title">
                    <span>Manage Budgets</span>
                    <button class="btn btn-primary" onclick="showBudgetModal()">
                        <i class="fas fa-edit"></i> Edit Budgets
                    </button>
                </div>
                <div id="budgetsList"></div>
            </div>
            
            <div class="card">
                <div class="card-title">
                    <span>Budget vs Actual</span>
                </div>
                <canvas id="budgetChart"></canvas>
            </div>
        </div>

        <!-- Calendar Tab -->
        <div id="calendar" class="tab-content">
            <div class="calendar-container">
                <div class="calendar-header">
                    <button class="month-btn" onclick="changeMonth(-1)"><i class="fas fa-chevron-left"></i></button>
                    <div class="month-display" id="calendarMonth">January 2024</div>
                    <button class="month-btn" onclick="changeMonth(1)"><i class="fas fa-chevron-right"></i></button>
                </div>
                
                <div class="calendar-grid">
                    <div class="calendar-day-header">Sun</div>
                    <div class="calendar-day-header">Mon</div>
                    <div class="calendar-day-header">Tue</div>
                    <div class="calendar-day-header">Wed</div>
                    <div class="calendar-day-header">Thu</div>
                    <div class="calendar-day-header">Fri</div>
                    <div class="calendar-day-header">Sat</div>
                </div>
                
                <div class="calendar-grid" id="calendarGrid"></div>
            </div>
            
            <div class="card" id="calendarExpenses">
                <div class="card-title">Daily Expenses</div>
                <div id="dayExpensesList" class="scrollable" style="max-height: 300px;"></div>
            </div>
        </div>

        <!-- To-Buy List Tab -->
        <div id="todo" class="tab-content">
            <div class="card">
                <div class="card-title">
                    <span>To-Buy List</span>
                    <button class="btn btn-primary" onclick="showTodoModal()">
                        <i class="fas fa-plus"></i> Add Item
                    </button>
                </div>
                <div id="todoList" class="scrollable" style="max-height: 400px;"></div>
            </div>
            
            <div class="card">
                <div class="card-title">
                    <span>To-Buy Statistics</span>
                </div>
                <div class="d-flex justify-between">
                    <div class="insight-card flex-1">
                        <div class="insight-title">Total Cost</div>
                        <div class="insight-value" id="todoTotalCost">0 AED</div>
                    </div>
                    <div class="insight-card flex-1">
                        <div class="insight-title">Items</div>
                        <div class="insight-value" id="todoItemCount">0</div>
                    </div>
                    <div class="insight-card flex-1">
                        <div class="insight-title">Completed</div>
                        <div class="insight-value" id="todoCompleted">0%</div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Goals Tab -->
        <div id="goals" class="tab-content">
            <div class="card">
                <div class="card-title">
                    <span>Financial Goals</span>
                    <button class="btn btn-primary" onclick="showGoalModal()">
                        <i class="fas fa-plus"></i> Add Goal
                    </button>
                </div>
                <div class="goals-container" id="goalsList"></div>
            </div>
        </div>

        <!-- Profiles Tab -->
        <div id="profiles" class="tab-content">
            <div class="card">
                <div class="card-title">
                    <span>Profile Management</span>
                </div>
                
                <div class="profile-stats">
                    <div class="profile-stat-card malek">
                        <div class="stat-label">Malek</div>
                        <div class="stat-value" id="malekTotalSpending">0 AED</div>
                        <div class="stat-label">Total Spending</div>
                    </div>
                    <div class="profile-stat-card sabrina">
                        <div class="stat-label">Sabrina</div>
                        <div class="stat-value" id="sabrinaTotalSpending">0 AED</div>
                        <div class="stat-label">Total Spending</div>
                    </div>
                </div>
                
                <div class="card mt-15">
                    <div class="card-title">Profile Balances</div>
                    <div class="form-group">
                        <label class="form-label">Malek's Balance (AED)</label>
                        <input type="number" class="form-input" id="malekBalance" value="5000">
                    </div>
                    <div class="form-group">
                        <label class="form-label">Sabrina's Balance (AED)</label>
                        <input type="number" class="form-input" id="sabrinaBalance" value="5000">
                    </div>
                    <button class="btn btn-primary w-100" onclick="updateProfileBalances()">
                        <i class="fas fa-save"></i> Update Balances
                    </button>
                </div>
            </div>
        </div>

        <!-- Settings Tab -->
        <div id="settings" class="tab-content">
            <div class="card">
                <div class="card-title">Category Management</div>
                <div id="categoryManager"></div>
                <button class="btn btn-secondary w-100 mt-15" onclick="showCategoryModal()">
                    <i class="fas fa-plus"></i> Add Category
                </button>
            </div>
            
            <div class="card">
                <div class="card-title">Data Management</div>
                <div class="d-flex gap-10 mb-15">
                    <button class="btn btn-secondary flex-1" onclick="exportAllData()">
                        <i class="fas fa-download"></i> Export All
                    </button>
                    <button class="btn btn-danger flex-1" onclick="importData()">
                        <i class="fas fa-upload"></i> Import
                    </button>
                </div>
                <button class="btn btn-danger w-100" onclick="clearAllData()">
                    <i class="fas fa-trash"></i> Clear All Data
                </button>
            </div>
            
            <div class="card">
                <div class="card-title">Backup & Sync</div>
                <div class="text-muted mb-15">
                    Data is automatically saved to your browser's storage.
                </div>
                <input type="file" id="backupFile" accept=".json" style="display: none;" onchange="restoreBackup(this)">
                <button class="btn btn-primary w-100 mb-10" onclick="document.getElementById('backupFile').click()">
                    <i class="fas fa-file-import"></i> Restore Backup
                </button>
                <button class="btn btn-secondary w-100" onclick="createBackup()">
                    <i class="fas fa-file-export"></i> Create Backup
                </button>
            </div>
        </div>
    </div>

    <!-- Quick Add Expense Section (Fixed at bottom) -->
    <div class="quick-add-section">
        <div class="quick-inputs">
            <input type="number" 
                   class="amount-input" 
                   id="quickAmount" 
                   placeholder="0.00" 
                   step="0.01"
                   autofocus
                   onkeydown="if(event.key === 'Enter') saveQuickExpense()">
            
            <select class="currency-select" id="quickCurrency">
                <option value="AED">🇦🇪 AED</option>
                <option value="DZD">🇩🇿 DZD</option>
            </select>
        </div>
        
        <select class="category-select" id="quickCategory"></select>
        <select class="profile-select" id="quickProfile">
            <option value="malek">👨 Malek</option>
            <option value="sabrina">👩 Sabrina</option>
        </select>
        
        <div class="quick-actions">
            <button class="quick-btn save-btn" onclick="saveQuickExpense()">
                <i class="fas fa-check"></i> ADD
            </button>
            <button class="quick-btn add-btn" onclick="showAddReceiptModal()">
                <i class="fas fa-camera"></i> DETAILS
            </button>
        </div>
    </div>

    <!-- Modals -->
    <!-- Add Expense Modal -->
    <div id="expenseModal" class="modal">
        <div class="modal-content">
            <div class="modal-header">
                <div class="modal-title">Add Expense</div>
                <button class="close-modal" onclick="closeModal('expenseModal')">&times;</button>
            </div>
            
            <div class="form-group">
                <label class="form-label">Description</label>
                <input type="text" id="expenseDescription" class="form-input" placeholder="What did you buy?">
            </div>
            
            <div class="form-group">
                <label class="form-label">Amount</label>
                <input type="number" id="expenseAmount" class="form-input" placeholder="0.00" step="0.01">
            </div>
            
            <div class="form-group">
                <label class="form-label">Currency</label>
                <select id="expenseCurrency" class="form-input">
                    <option value="AED">AED</option>
                    <option value="DZD">DZD</option>
                </select>
            </div>
            
            <div class="form-group">
                <label class="form-label">Category</label>
                <select id="expenseCategory" class="form-input"></select>
            </div>
            
            <div class="form-group">
                <label class="form-label">Profile</label>
                <select id="expenseProfile" class="form-input">
                    <option value="malek">👨 Malek</option>
                    <option value="sabrina">👩 Sabrina</option>
                </select>
            </div>
            
            <button class="btn btn-primary w-100" onclick="saveExpense()">
                <i class="fas fa-save"></i> Save Expense
            </button>
        </div>
    </div>

    <!-- Budget Modal -->
    <div id="budgetModal" class="modal">
        <div class="modal-content">
            <div class="modal-header">
                <div class="modal-title">Edit Budgets</div>
                <button class="close-modal" onclick="closeModal('budgetModal')">&times;</button>
            </div>
            
            <div id="budgetEditList"></div>
            
            <button class="btn btn-primary w-100" onclick="saveAllBudgets()">
                <i class="fas fa-save"></i> Save All Budgets
            </button>
        </div>
    </div>

    <!-- To-Do Modal -->
    <div id="todoModal" class="modal">
        <div class="modal-content">
            <div class="modal-header">
                <div class="modal-title">Add To-Buy Item</div>
                <button class="close-modal" onclick="closeModal('todoModal')">&times;</button>
            </div>
            
            <div class="form-group">
                <label class="form-label">Item Name</label>
                <input type="text" id="todoName" class="form-input" placeholder="What to buy?">
            </div>
            
            <div class="form-group">
                <label class="form-label">Category</label>
                <select id="todoCategory" class="form-input">
                    <option value="">Select category</option>
                </select>
            </div>
            
            <div class="form-group">
                <label class="form-label">Estimated Cost (AED)</label>
                <input type="number" id="todoCost" class="form-input" placeholder="0.00" step="0.01">
            </div>
            
            <div class="form-group">
                <label class="form-label">Profile</label>
                <select id="todoProfile" class="form-input">
                    <option value="malek">👨 Malek</option>
                    <option value="sabrina">👩 Sabrina</option>
                </select>
            </div>
            
            <div class="form-group">
                <label class="form-label">Priority</label>
                <select id="todoPriority" class="form-input">
                    <option value="low">Low</option>
                    <option value="medium">Medium</option>
                    <option value="high">High</option>
                </select>
            </div>
            
            <button class="btn btn-primary w-100" onclick="saveTodoItem()">
                <i class="fas fa-save"></i> Add to List
            </button>
        </div>
    </div>

    <!-- Goal Modal -->
    <div id="goalModal" class="modal">
        <div class="modal-content">
            <div class="modal-header">
                <div class="modal-title">Add Financial Goal</div>
                <button class="close-modal" onclick="closeModal('goalModal')">&times;</button>
            </div>
            
            <div class="form-group">
                <label class="form-label">Goal Title</label>
                <input type="text" id="goalTitle" class="form-input" placeholder="e.g., Save for Vacation">
            </div>
            
            <div class="form-group">
                <label class="form-label">Target Amount (AED)</label>
                <input type="number" id="goalTarget" class="form-input" placeholder="0.00" step="0.01">
            </div>
            
            <div class="form-group">
                <label class="form-label">Current Amount (AED)</label>
                <input type="number" id="goalCurrent" class="form-input" placeholder="0.00" step="0.01">
            </div>
            
            <div class="form-group">
                <label class="form-label">Target Date</label>
                <input type="date" id="goalDate" class="form-input">
            </div>
            
            <div class="form-group">
                <label class="form-label">Profile</label>
                <select id="goalProfile" class="form-input">
                    <option value="both">Both</option>
                    <option value="malek">Malek</option>
                    <option value="sabrina">Sabrina</option>
                </select>
            </div>
            
            <div class="form-group">
                <label class="form-label">Priority</label>
                <select id="goalPriority" class="form-input">
                    <option value="low">Low</option>
                    <option value="medium">Medium</option>
                    <option value="high">High</option>
                </select>
            </div>
            
            <div class="form-group">
                <label class="form-label">Description (Optional)</label>
                <textarea id="goalDescription" class="form-input" rows="3" placeholder="Describe your goal..."></textarea>
            </div>
            
            <button class="btn btn-primary w-100" onclick="saveGoal()">
                <i class="fas fa-save"></i> Save Goal
            </button>
        </div>
    </div>

    <!-- Category Modal -->
    <div id="categoryModal" class="modal">
        <div class="modal-content">
            <div class="modal-header">
                <div class="modal-title">Manage Categories</div>
                <button class="close-modal" onclick="closeModal('categoryModal')">&times;</button>
            </div>
            
            <div id="categoryEditList" class="mb-15"></div>
            
            <div class="form-group">
                <label class="form-label">Add New Category</label>
                <input type="text" id="newCategoryName" class="form-input" placeholder="e.g., Groceries">
            </div>
            
            <div class="form-group">
                <label class="form-label">Default Monthly Budget (AED)</label>
                <input type="number" id="categoryBudget" class="form-input" placeholder="500" step="0.01">
            </div>
            
            <button class="btn btn-primary w-100" onclick="saveNewCategory()">
                <i class="fas fa-save"></i> Save Category
            </button>
        </div>
    </div>

    <!-- Expense Detail Modal -->
    <div id="expenseDetailModal" class="modal">
        <div class="modal-content">
            <div class="modal-header">
                <div class="modal-title">Expense Details</div>
                <button class="close-modal" onclick="closeModal('expenseDetailModal')">&times;</button>
            </div>
            <div id="expenseDetailContent"></div>
        </div>
    </div>

    <!-- Notification -->
    <div id="notification" style="display: none; position: fixed; top: 20px; right: 20px; background: linear-gradient(135deg, #D4AF37, #B8860B); color: #000; padding: 15px; border-radius: var(--radius); box-shadow: 0 4px 20px rgba(212, 175, 55, 0.3); z-index: 3000; max-width: 300px; border: 1px solid rgba(212, 175, 55, 0.5);">
        Expense added successfully!
    </div>

    <script>
        // ========== GLOBAL CONFIGURATION ==========
        const EXCHANGE_RATE = 65; // 1 AED = 65 DZD
        
        // Default Categories
        const DEFAULT_CATEGORIES = [
            { id: 'food', name: 'Food', icon: '🍔', color: '#FF6B6B', budget: 1500 },
            { id: 'bills', name: 'Bills', icon: '💡', color: '#4ECDC4', budget: 1100 },
            { id: 'entertainment', name: 'Entertainment', icon: '🎬', color: '#FFD166', budget: 400 },
            { id: 'household', name: 'Household', icon: '🏠', color: '#06D6A0', budget: 500 },
            { id: 'car', name: 'Car', icon: '🚗', color: '#118AB2', budget: 7000 },
            { id: 'flights', name: 'Flights', icon: '✈️', color: '#073B4C', budget: 0 },
            { id: 'health', name: 'Health', icon: '🏥', color: '#EF476F', budget: 0 },
            { id: 'shopping', name: 'Shopping', icon: '🛍️', color: '#7209B7', budget: 1000 },
            { id: 'savings', name: 'Savings', icon: '💰', color: '#F9C74F', budget: 2000 },
            { id: 'other', name: 'Other', icon: '📦', color: '#6B7280', budget: 500 }
        ];

        // Profiles
        const PROFILES = {
            malek: {
                id: 'malek',
                name: 'Malek',
                color: '#3498db',
                icon: '👨',
                balance: 5000
            },
            sabrina: {
                id: 'sabrina',
                name: 'Sabrina',
                color: '#e74c3c',
                icon: '👩',
                balance: 5000
            }
        };

        // ========== GLOBAL STATE ==========
        let expenses = [];
        let budgets = [];
        let categories = [];
        let todoItems = [];
        let goals = [];
        let currentMonth = new Date().getMonth();
        let currentYear = new Date().getFullYear();
        let filteredExpenses = [];
        let currentProfile = 'malek'; // Default profile

        // ========== INITIALIZATION ==========
        document.addEventListener('DOMContentLoaded', function() {
            loadAllData();
            initializeApp();
            updateAllDisplays();
            
            // Set current month display
            const monthNames = ['January', 'February', 'March', 'April', 'May', 'June',
                              'July', 'August', 'September', 'October', 'November', 'December'];
            document.getElementById('currentMonth').textContent = 
                `${monthNames[currentMonth]} ${currentYear}`;
        });

        function initializeApp() {
            // Initialize categories
            const savedCategories = localStorage.getItem('makkbenCategories');
            if (savedCategories) {
                categories = JSON.parse(savedCategories);
            } else {
                categories = [...DEFAULT_CATEGORIES];
                saveCategories();
            }
            
            // Initialize profile balances
            const savedBalances = localStorage.getItem('makkbenProfileBalances');
            if (savedBalances) {
                const balances = JSON.parse(savedBalances);
                PROFILES.malek.balance = balances.malek || 5000;
                PROFILES.sabrina.balance = balances.sabrina || 5000;
                document.getElementById('malekBalance').value = PROFILES.malek.balance;
                document.getElementById('sabrinaBalance').value = PROFILES.sabrina.balance;
            }
            
            // Ensure all categories have budgets
            ensureAllCategoriesHaveBudgets();
            
            // Load categories into selects
            updateCategorySelects();
            populateFilterCategories();
            populateMonthFilter();
            
            // Update UI for current profile
            updateProfileUI();
        }

        // ========== PROFILE MANAGEMENT ==========
        function switchProfile(profileId) {
            // Update active profile buttons
            document.querySelectorAll('.profile-btn').forEach(btn => {
                btn.classList.remove('active');
            });
            document.querySelector(`.profile-btn.${profileId}`).classList.add('active');
            
            // Update current profile
            currentProfile = profileId;
            
            // Update UI
            updateProfileUI();
            
            // Update displays
            updateAllDisplays();
        }

        function updateProfileUI() {
            const profile = PROFILES[currentProfile];
            
            // Update avatar and name
            document.getElementById('currentAvatar').className = `user-avatar avatar-${currentProfile}`;
            document.getElementById('currentAvatar').textContent = profile.name.charAt(0);
            document.getElementById('currentUserName').textContent = profile.name;
            document.getElementById('currentUserEmail').textContent = `${profile.name}'s Expenses`;
            
            // Update quick profile selector
            document.getElementById('quickProfile').value = currentProfile;
        }

        function updateProfileBalances() {
            const malekBalance = parseFloat(document.getElementById('malekBalance').value) || 0;
            const sabrinaBalance = parseFloat(document.getElementById('sabrinaBalance').value) || 0;
            
            PROFILES.malek.balance = malekBalance;
            PROFILES.sabrina.balance = sabrinaBalance;
            
            localStorage.setItem('makkbenProfileBalances', JSON.stringify({
                malek: malekBalance,
                sabrina: sabrinaBalance
            }));
            
            updateAllDisplays();
            showNotification('Profile balances updated');
        }

        function getProfileSpending(profileId) {
            const monthExpenses = getMonthExpenses();
            return monthExpenses
                .filter(exp => exp.profile === profileId)
                .reduce((sum, exp) => sum + convertAmount(exp.amount, exp.currency, 'AED'), 0);
        }

        function getTotalProfileSpending(profileId) {
            return expenses
                .filter(exp => exp.profile === profileId)
                .reduce((sum, exp) => sum + convertAmount(exp.amount, exp.currency, 'AED'), 0);
        }

        // ========== DATA MANAGEMENT ==========
        function loadAllData() {
            try {
                // Load expenses
                const savedExpenses = localStorage.getItem('makkbenExpenses');
                expenses = savedExpenses ? JSON.parse(savedExpenses) : [];
                filteredExpenses = [...expenses];
                
                // Load budgets
                const savedBudgets = localStorage.getItem('makkbenBudgets');
                budgets = savedBudgets ? JSON.parse(savedBudgets) : [];
                
                // Load todo items
                const savedTodos = localStorage.getItem('makkbenTodos');
                todoItems = savedTodos ? JSON.parse(savedTodos) : [];
                
                // Load goals
                const savedGoals = localStorage.getItem('makkbenGoals');
                goals = savedGoals ? JSON.parse(savedGoals) : [];
                
            } catch (error) {
                console.error('Error loading data:', error);
                showNotification('Error loading data', 'error');
            }
        }

        function saveAllData() {
            try {
                localStorage.setItem('makkbenExpenses', JSON.stringify(expenses));
                localStorage.setItem('makkbenBudgets', JSON.stringify(budgets));
                localStorage.setItem('makkbenTodos', JSON.stringify(todoItems));
                localStorage.setItem('makkbenCategories', JSON.stringify(categories));
                localStorage.setItem('makkbenGoals', JSON.stringify(goals));
            } catch (error) {
                console.error('Error saving data:', error);
                showNotification('Error saving data', 'error');
            }
        }

        function saveCategories() {
            localStorage.setItem('makkbenCategories', JSON.stringify(categories));
        }

        function ensureAllCategoriesHaveBudgets() {
            categories.forEach(category => {
                const existingBudget = budgets.find(b => b.categoryId === category.id);
                if (!existingBudget) {
                    const budgetAmount = category.budget || 500;
                    budgets.push({
                        id: Date.now() + Math.random(),
                        categoryId: category.id,
                        categoryName: category.name,
                        amount: budgetAmount,
                        period: 'monthly',
                        spent: 0,
                        createdAt: new Date().toISOString()
                    });
                }
            });
            saveAllData();
        }

        // ========== UI UPDATES ==========
        function updateAllDisplays() {
            updateDashboard();
            updateExpensesList();
            updateBudgetsList();
            updateBudgetOverview();
            updateTodoList();
            updateTodoStats();
            updateCalendar();
            updateQuickStats();
            updateGoalsList();
            updateRecentExpenses();
            updateProfileStats();
            updateCategoryManager();
        }

        function updateQuickStats() {
            const monthExpenses = getMonthExpenses();
            const monthTotal = monthExpenses.reduce((sum, exp) => 
                sum + convertAmount(exp.amount, exp.currency, 'AED'), 0);
            
            const currentBalance = PROFILES[currentProfile].balance;
            const remaining = currentBalance - getProfileSpending(currentProfile);
            
            document.getElementById('totalBalance').textContent = 
                formatCurrency(currentBalance, 'AED');
            document.getElementById('monthExpenses').textContent = 
                formatCurrency(monthTotal, 'AED');
            document.getElementById('remainingBalance').textContent = 
                formatCurrency(remaining, 'AED');
            
            const remainingElem = document.getElementById('remainingBalance');
            if (remaining < 0) {
                remainingElem.classList.add('budget-warning');
            } else if (remaining < 1000) {
                remainingElem.classList.add('budget-close');
            } else {
                remainingElem.classList.remove('budget-warning', 'budget-close');
            }
        }

        function updateProfileStats() {
            // Update month spending
            document.getElementById('malekMonthSpending').textContent = 
                formatCurrency(getProfileSpending('malek'), 'AED');
            document.getElementById('sabrinaMonthSpending').textContent = 
                formatCurrency(getProfileSpending('sabrina'), 'AED');
            
            // Update total spending
            document.getElementById('malekTotalSpending').textContent = 
                formatCurrency(getTotalProfileSpending('malek'), 'AED');
            document.getElementById('sabrinaTotalSpending').textContent = 
                formatCurrency(getTotalProfileSpending('sabrina'), 'AED');
        }

        function updateRecentExpenses() {
            const container = document.getElementById('recentExpenses');
            if (!container) return;
            
            const recent = expenses.slice(0, 5);
            
            if (recent.length === 0) {
                container.innerHTML = '<div class="text-muted">No recent expenses</div>';
                return;
            }
            
            container.innerHTML = recent.map(exp => {
                const category = categories.find(c => c.id === exp.categoryId) || {};
                return `
                    <div class="expense-item">
                        <div class="expense-icon" style="background: linear-gradient(135deg, ${category.color || '#D4AF37'}, #FFD700)">
                            ${category.icon || '📦'}
                        </div>
                        <div class="expense-details">
                            <div class="expense-title truncate">${exp.description}</div>
                            <div class="expense-meta">
                                <span>${exp.date}</span>
                                <span>•</span>
                                <span>${category.name}</span>
                                <span class="user-badge ${exp.profile}">${exp.profile === 'malek' ? '👨' : '👩'} ${exp.profile}</span>
                            </div>
                        </div>
                        <div class="expense-amount">
                            <div class="amount-primary truncate">${formatCurrency(exp.amount, exp.currency)}</div>
                        </div>
                    </div>
                `;
            }).join('');
        }

        // ========== EXPENSE MANAGEMENT ==========
        function saveQuickExpense() {
            const amountInput = document.getElementById('quickAmount');
            const categorySelect = document.getElementById('quickCategory');
            const currencySelect = document.getElementById('quickCurrency');
            const profileSelect = document.getElementById('quickProfile');
            
            const amount = parseFloat(amountInput.value);
            const categoryId = categorySelect.value;
            const currency = currencySelect.value;
            const profile = profileSelect.value;
            
            if (!amount || amount <= 0) {
                showNotification('Please enter a valid amount', 'error');
                return;
            }
            
            if (!categoryId) {
                showNotification('Please select a category', 'error');
                return;
            }
            
            const category = categories.find(c => c.id === categoryId);
            const now = new Date();
            
            const expense = {
                id: Date.now(),
                amount: amount,
                currency: currency,
                description: `Quick Expense - ${category.name}`,
                categoryId: categoryId,
                categoryName: category.name,
                categoryIcon: category.icon,
                categoryColor: category.color,
                profile: profile,
                date: now.toISOString().split('T')[0],
                time: now.toLocaleTimeString([], { hour: '2-digit', minute: '2-digit' }),
                timestamp: now.getTime(),
                hasReceipt: false,
                createdAt: now.toISOString()
            };
            
            expenses.unshift(expense);
            filteredExpenses.unshift(expense);
            
            // Update profile balance
            PROFILES[profile].balance -= convertAmount(amount, currency, 'AED');
            saveProfileBalances();
            
            // Update budget
            updateBudgetSpending(categoryId, convertAmount(amount, currency, 'AED'));
            
            saveAllData();
            updateAllDisplays();
            filterExpenses();
            
            amountInput.value = '';
            amountInput.focus();
            
            showNotification(`${category.icon} ${amount.toFixed(2)} ${currency} added for ${PROFILES[profile].name}`);
        }

        function showAddReceiptModal() {
            const categorySelect = document.getElementById('expenseCategory');
            categorySelect.innerHTML = '<option value="">Select category</option>';
            
            categories.forEach(cat => {
                const option = document.createElement('option');
                option.value = cat.id;
                option.textContent = `${cat.icon} ${cat.name}`;
                categorySelect.appendChild(option);
            });
            
            openModal('expenseModal');
        }

        function saveExpense() {
            const description = document.getElementById('expenseDescription').value;
            const amount = parseFloat(document.getElementById('expenseAmount').value);
            const currency = document.getElementById('expenseCurrency').value;
            const categoryId = document.getElementById('expenseCategory').value;
            const profile = document.getElementById('expenseProfile').value;
            
            if (!amount || amount <= 0) {
                showNotification('Please enter a valid amount', 'error');
                return;
            }
            
            if (!categoryId) {
                showNotification('Please select a category', 'error');
                return;
            }
            
            const category = categories.find(c => c.id === categoryId);
            const now = new Date();
            
            const expense = {
                id: Date.now(),
                amount: amount,
                currency: currency,
                description: description || `Expense - ${category.name}`,
                categoryId: categoryId,
                categoryName: category.name,
                categoryIcon: category.icon,
                categoryColor: category.color,
                profile: profile,
                date: now.toISOString().split('T')[0],
                time: now.toLocaleTimeString([], { hour: '2-digit', minute: '2-digit' }),
                timestamp: now.getTime(),
                hasReceipt: false,
                createdAt: now.toISOString()
            };
            
            expenses.unshift(expense);
            filteredExpenses.unshift(expense);
            
            // Update profile balance
            PROFILES[profile].balance -= convertAmount(amount, currency, 'AED');
            saveProfileBalances();
            
            // Update budget
            updateBudgetSpending(category.id, convertAmount(amount, currency, 'AED'));
            
            saveAllData();
            updateAllDisplays();
            filterExpenses();
            
            // Clear form
            document.getElementById('expenseDescription').value = '';
            document.getElementById('expenseAmount').value = '';
            document.getElementById('expenseCategory').selectedIndex = 0;
            
            closeModal('expenseModal');
            showNotification(`Expense saved for ${PROFILES[profile].name}`);
        }

        function deleteExpense(expenseId) {
            const expense = expenses.find(e => e.id === expenseId);
            if (!expense) return;
            
            if (confirm('Delete this expense?')) {
                // Add back to profile balance
                PROFILES[expense.profile].balance += convertAmount(expense.amount, expense.currency, 'AED');
                saveProfileBalances();
                
                // Remove from budget spending
                const budget = budgets.find(b => b.categoryId === expense.categoryId);
                if (budget) {
                    budget.spent = Math.max(0, budget.spent - convertAmount(expense.amount, expense.currency, 'AED'));
                }
                
                expenses = expenses.filter(e => e.id !== expenseId);
                filteredExpenses = filteredExpenses.filter(e => e.id !== expenseId);
                
                saveAllData();
                updateAllDisplays();
                showNotification('Expense deleted');
            }
        }

        function editExpense(expenseId) {
            const expense = expenses.find(e => e.id === expenseId);
            if (!expense) return;
            
            showAddReceiptModal();
            
            // Pre-fill form
            setTimeout(() => {
                document.getElementById('expenseDescription').value = expense.description;
                document.getElementById('expenseAmount').value = expense.amount;
                document.getElementById('expenseCurrency').value = expense.currency;
                document.getElementById('expenseCategory').value = expense.categoryId;
                document.getElementById('expenseProfile').value = expense.profile;
                
                // Change save button to update
                const saveBtn = document.querySelector('#expenseModal .btn-primary');
                saveBtn.innerHTML = '<i class="fas fa-save"></i> Update Expense';
                saveBtn.onclick = () => updateExpense(expenseId);
            }, 100);
        }

        function updateExpense(expenseId) {
            const expenseIndex = expenses.findIndex(e => e.id === expenseId);
            if (expenseIndex === -1) return;
            
            const oldExpense = expenses[expenseIndex];
            const description = document.getElementById('expenseDescription').value;
            const amount = parseFloat(document.getElementById('expenseAmount').value);
            const currency = document.getElementById('expenseCurrency').value;
            const categoryId = document.getElementById('expenseCategory').value;
            const profile = document.getElementById('expenseProfile').value;
            const category = categories.find(c => c.id === categoryId);
            
            if (!amount || amount <= 0) {
                showNotification('Please enter a valid amount', 'error');
                return;
            }
            
            if (!categoryId) {
                showNotification('Please select a category', 'error');
                return;
            }
            
            // Adjust profile balance
            const oldAmountInAED = convertAmount(oldExpense.amount, oldExpense.currency, 'AED');
            const newAmountInAED = convertAmount(amount, currency, 'AED');
            
            PROFILES[oldExpense.profile].balance += oldAmountInAED;
            PROFILES[profile].balance -= newAmountInAED;
            saveProfileBalances();
            
            // Adjust old budget
            const oldBudget = budgets.find(b => b.categoryId === oldExpense.categoryId);
            if (oldBudget) {
                oldBudget.spent = Math.max(0, oldBudget.spent - oldAmountInAED);
            }
            
            // Update expense
            expenses[expenseIndex] = {
                ...oldExpense,
                amount: amount,
                currency: currency,
                description: description,
                categoryId: categoryId,
                categoryName: category.name,
                categoryIcon: category.icon,
                categoryColor: category.color,
                profile: profile,
                updatedAt: new Date().toISOString()
            };
            
            // Update new budget
            updateBudgetSpending(categoryId, newAmountInAED);
            
            filteredExpenses = [...expenses];
            saveAllData();
            updateAllDisplays();
            
            closeModal('expenseModal');
            showNotification('Expense updated');
        }

        function saveProfileBalances() {
            localStorage.setItem('makkbenProfileBalances', JSON.stringify({
                malek: PROFILES.malek.balance,
                sabrina: PROFILES.sabrina.balance
            }));
        }

        // ========== UTILITY FUNCTIONS ==========
        function formatCurrency(amount, currency) {
            const formatted = amount.toLocaleString(undefined, {
                minimumFractionDigits: 0,
                maximumFractionDigits: 0
            });
            
            if (currency === 'DZD' && amount > 10000) {
                return formatted.replace(/,/g, ' ') + ' ' + currency;
            }
            
            return formatted + ' ' + currency;
        }

        function convertAmount(amount, fromCurrency, toCurrency) {
            if (fromCurrency === toCurrency) return amount;
            
            if (fromCurrency === 'AED' && toCurrency === 'DZD') {
                return amount * EXCHANGE_RATE;
            } else if (fromCurrency === 'DZD' && toCurrency === 'AED') {
                return amount / EXCHANGE_RATE;
            }
            return amount;
        }

        function getMonthExpenses() {
            const now = new Date();
            const currentMonth = now.getMonth();
            const currentYear = now.getFullYear();
            
            return expenses.filter(exp => {
                const expDate = new Date(exp.timestamp);
                return expDate.getMonth() === currentMonth && 
                       expDate.getFullYear() === currentYear;
            });
        }

        function switchTab(tabId) {
            // Update active tab
            document.querySelectorAll('.nav-tab').forEach(tab => {
                tab.classList.remove('active');
            });
            document.querySelectorAll(`[onclick*="${tabId}"]`).forEach(tab => {
                tab.classList.add('active');
            });
            
            // Update content
            document.querySelectorAll('.tab-content').forEach(content => {
                content.classList.remove('active');
            });
            document.getElementById(tabId).classList.add('active');
        }

        function openModal(modalId) {
            document.getElementById(modalId).classList.add('active');
        }

        function closeModal(modalId) {
            document.getElementById(modalId).classList.remove('active');
        }

        function showNotification(message, type = 'success') {
            const notification = document.getElementById('notification');
            if (!notification) return;
            
            notification.textContent = message;
            notification.style.background = type === 'error' ? 'linear-gradient(135deg, #C41E3A, #A8152F)' : 
                                           type === 'info' ? 'linear-gradient(135deg, #FFA500, #F59E0B)' : 
                                           'linear-gradient(135deg, #D4AF37, #B8860B)';
            notification.style.display = 'block';
            
            setTimeout(() => {
                notification.style.display = 'none';
            }, 3000);
        }

        // ========== EXPENSE LIST ==========
        function filterExpenses() {
            const categoryFilter = document.getElementById('filterCategory').value;
            const monthFilter = document.getElementById('filterMonth').value;
            const currencyFilter = document.getElementById('filterCurrency').value;
            const profileFilter = document.getElementById('filterProfile').value;
            
            filteredExpenses = expenses.filter(exp => {
                // Category filter
                if (categoryFilter && exp.categoryId !== categoryFilter) return false;
                
                // Month filter
                if (monthFilter) {
                    const expDate = new Date(exp.timestamp);
                    const filterDate = new Date(monthFilter);
                    if (expDate.getMonth() !== filterDate.getMonth() || 
                        expDate.getFullYear() !== filterDate.getFullYear()) {
                        return false;
                    }
                }
                
                // Currency filter
                if (currencyFilter && exp.currency !== currencyFilter) return false;
                
                // Profile filter
                if (profileFilter && exp.profile !== profileFilter) return false;
                
                return true;
            });
            
            updateFilteredStats();
            updateExpensesList();
        }

        function updateFilteredStats() {
            const total = filteredExpenses.reduce((sum, exp) => 
                sum + convertAmount(exp.amount, exp.currency, 'AED'), 0);
            
            document.getElementById('filteredTotal').textContent = formatCurrency(total, 'AED');
            document.getElementById('filteredCount').textContent = filteredExpenses.length;
        }

        function updateExpensesList() {
            const container = document.getElementById('expensesList');
            if (!container) return;
            
            if (filteredExpenses.length === 0) {
                container.innerHTML = `
                    <div class="loading">
                        <i class="fas fa-receipt"></i>
                        <div class="text-muted mt-10">No expenses found</div>
                    </div>
                `;
                return;
            }
            
            container.innerHTML = filteredExpenses.map(expense => {
                const category = categories.find(c => c.id === expense.categoryId) || {};
                const amountInAED = convertAmount(expense.amount, expense.currency, 'AED');
                const amountInDZD = convertAmount(expense.amount, expense.currency, 'DZD');
                
                return `
                    <div class="expense-item">
                        <div class="expense-icon" style="background: linear-gradient(135deg, ${category.color || '#D4AF37'}, #FFD700)">
                            ${category.icon || '📦'}
                        </div>
                        <div class="expense-details">
                            <div class="expense-title truncate">${expense.description}</div>
                            <div class="expense-meta">
                                <span>${expense.date}</span>
                                <span>•</span>
                                <span>${expense.time}</span>
                                <span>•</span>
                                <span>${category.name}</span>
                                <span class="user-badge ${expense.profile}">${expense.profile === 'malek' ? '👨' : '👩'} ${expense.profile}</span>
                            </div>
                        </div>
                        <div class="expense-amount">
                            <div class="amount-primary truncate">${formatCurrency(expense.amount, expense.currency)}</div>
                            <div class="amount-secondary truncate">
                                ≈ ${formatCurrency(amountInAED, 'AED')}
                                ${expense.currency !== 'DZD' ? `<br>≈ ${formatCurrency(amountInDZD, 'DZD')}` : ''}
                            </div>
                        </div>
                        <div class="item-actions">
                            <button class="btn btn-secondary btn-sm" onclick="editExpense(${expense.id})">
                                <i class="fas fa-edit"></i>
                            </button>
                            <button class="btn btn-danger btn-sm" onclick="deleteExpense(${expense.id})">
                                <i class="fas fa-trash"></i>
                            </button>
                        </div>
                    </div>
                `;
            }).join('');
        }

        // ========== DASHBOARD CHART ==========
        function updateDashboard() {
            updateDashboardChart();
        }

        function updateDashboardChart() {
            const ctx = document.getElementById('dashboardChart');
            if (!ctx) return;
            
            const monthExpenses = getMonthExpenses();
            const categoryTotals = {};
            
            monthExpenses.forEach(exp => {
                const amountInAED = convertAmount(exp.amount, exp.currency, 'AED');
                if (!categoryTotals[exp.categoryId]) {
                    categoryTotals[exp.categoryId] = 0;
                }
                categoryTotals[exp.categoryId] += amountInAED;
            });
            
            const labels = [];
            const data = [];
            const colors = [];
            
            Object.entries(categoryTotals).forEach(([categoryId, total]) => {
                const category = categories.find(c => c.id === categoryId);
                if (category && total > 0) {
                    labels.push(category.name);
                    data.push(total);
                    colors.push(category.color);
                }
            });
            
            if (window.dashboardChart instanceof Chart) {
                window.dashboardChart.destroy();
            }
            
            window.dashboardChart = new Chart(ctx, {
                type: 'doughnut',
                data: {
                    labels: labels,
                    datasets: [{
                        data: data,
                        backgroundColor: colors,
                        borderWidth: 2,
                        borderColor: '#1A1A1A'
                    }]
                },
                options: {
                    responsive: true,
                    maintainAspectRatio: false,
                    plugins: {
                        legend: {
                            position: 'bottom',
                            labels: {
                                padding: 15,
                                font: { size: 11 },
                                color: '#F5F5F5'
                            }
                        }
                    },
                    cutout: '60%'
                }
            });
        }

        // ========== CATEGORY MANAGEMENT ==========
        function updateCategorySelects() {
            const selects = [
                document.getElementById('quickCategory'),
                document.getElementById('expenseCategory'),
                document.getElementById('todoCategory')
            ];
            
            selects.forEach(select => {
                if (!select) return;
                
                select.innerHTML = '<option value="">Select category</option>';
                categories.forEach(cat => {
                    const option = document.createElement('option');
                    option.value = cat.id;
                    option.textContent = `${cat.icon} ${cat.name}`;
                    select.appendChild(option);
                });
            });
        }

        function populateFilterCategories() {
            const select = document.getElementById('filterCategory');
            select.innerHTML = '<option value="">All Categories</option>';
            
            categories.forEach(cat => {
                const option = document.createElement('option');
                option.value = cat.id;
                option.textContent = `${cat.icon} ${cat.name}`;
                select.appendChild(option);
            });
        }

        function populateMonthFilter() {
            const select = document.getElementById('filterMonth');
            select.innerHTML = '<option value="">All Time</option>';
            
            // Get unique months from expenses
            const months = new Set();
            expenses.forEach(exp => {
                const date = new Date(exp.timestamp);
                const monthStr = `${date.getFullYear()}-${(date.getMonth() + 1).toString().padStart(2, '0')}`;
                months.add(monthStr);
            });
            
            // Convert to array and sort descending
            const sortedMonths = Array.from(months).sort().reverse();
            
            sortedMonths.forEach(monthStr => {
                const [year, month] = monthStr.split('-');
                const date = new Date(year, month - 1);
                const option = document.createElement('option');
                option.value = `${year}-${month.padStart(2, '0')}-01`;
                option.textContent = date.toLocaleDateString('en-US', { month: 'long', year: 'numeric' });
                select.appendChild(option);
            });
        }

        function showCategoryModal() {
            const container = document.getElementById('categoryEditList');
            container.innerHTML = '';
            
            categories.forEach(category => {
                container.innerHTML += `
                    <div class="d-flex justify-between align-center mb-10 p-10" style="background: var(--background); border-radius: var(--radius);">
                        <div class="d-flex align-center gap-10">
                            <div style="font-size: 24px;">${category.icon}</div>
                            <div>
                                <div>${category.name}</div>
                                <div class="text-muted">${formatCurrency(category.budget || 0, 'AED')}</div>
                            </div>
                        </div>
                        <div class="d-flex gap-5">
                            <button class="btn btn-secondary btn-sm" onclick="editCategory('${category.id}')">
                                <i class="fas fa-edit"></i>
                            </button>
                            <button class="btn btn-danger btn-sm" onclick="deleteCategory('${category.id}')" ${category.id === 'other' ? 'disabled' : ''}>
                                <i class="fas fa-trash"></i>
                            </button>
                        </div>
                    </div>
                `;
            });
            
            openModal('categoryModal');
        }

        function editCategory(categoryId) {
            const category = categories.find(c => c.id === categoryId);
            if (!category) return;
            
            const newName = prompt('Enter new category name:', category.name);
            if (!newName) return;
            
            const newBudget = parseFloat(prompt('Enter new budget (AED):', category.budget || 0));
            if (isNaN(newBudget)) return;
            
            category.name = newName;
            category.budget = newBudget;
            
            // Update related budget
            const budget = budgets.find(b => b.categoryId === categoryId);
            if (budget) {
                budget.categoryName = newName;
                budget.amount = newBudget;
            }
            
            saveAllData();
            updateAllDisplays();
            showCategoryModal();
            showNotification('Category updated');
        }

        function deleteCategory(categoryId) {
            if (categoryId === 'other') {
                showNotification('Cannot delete "Other" category', 'error');
                return;
            }
            
            if (confirm('Delete this category? All related expenses will be moved to "Other" category.')) {
                // Move expenses to "other" category
                expenses.forEach(expense => {
                    if (expense.categoryId === categoryId) {
                        const otherCategory = categories.find(c => c.id === 'other');
                        expense.categoryId = 'other';
                        expense.categoryName = otherCategory.name;
                        expense.categoryIcon = otherCategory.icon;
                        expense.categoryColor = otherCategory.color;
                    }
                });
                
                // Remove category
                categories = categories.filter(c => c.id !== categoryId);
                
                // Remove budget
                budgets = budgets.filter(b => b.categoryId !== categoryId);
                
                saveAllData();
                updateAllDisplays();
                showCategoryModal();
                showNotification('Category deleted');
            }
        }

        function saveNewCategory() {
            const nameInput = document.getElementById('newCategoryName');
            const budgetInput = document.getElementById('categoryBudget');
            
            const name = nameInput.value.trim();
            const budget = parseFloat(budgetInput.value) || 500;
            
            if (!name) {
                showNotification('Please enter category name', 'error');
                return;
            }
            
            const id = name.toLowerCase().replace(/\s+/g, '_');
            
            if (categories.find(c => c.id === id)) {
                showNotification('Category already exists', 'error');
                return;
            }
            
            const icons = ['🍎', '🚗', '🏠', '💡', '🎬', '✈️', '🏥', '🛍️', '💰', '📦', '🍔', '🎯', '⭐', '👑'];
            const colors = ['#FF6B6B', '#4ECDC4', '#FFD166', '#06D6A0', '#118AB2', '#073B4C', '#EF476F', '#7209B7', '#F9C74F', '#6B7280'];
            
            const newCategory = {
                id: id,
                name: name,
                icon: icons[Math.floor(Math.random() * icons.length)],
                color: colors[Math.floor(Math.random() * colors.length)],
                budget: budget
            };
            
            categories.push(newCategory);
            
            budgets.push({
                id: Date.now(),
                categoryId: id,
                categoryName: name,
                amount: budget,
                period: 'monthly',
                spent: 0,
                createdAt: new Date().toISOString()
            });
            
            saveAllData();
            updateCategorySelects();
            populateFilterCategories();
            updateAllDisplays();
            
            nameInput.value = '';
            budgetInput.value = '';
            
            showCategoryModal();
            showNotification('Category added');
        }

        function updateCategoryManager() {
            const container = document.getElementById('categoryManager');
            if (!container) return;
            
            container.innerHTML = categories.map(cat => {
                const budget = budgets.find(b => b.categoryId === cat.id);
                const spent = budget?.spent || 0;
                const amount = budget?.amount || 0;
                const percentage = amount > 0 ? Math.min((spent / amount) * 100, 100) : 0;
                
                return `
                    <div class="d-flex justify-between align-center mb-10">
                        <div class="d-flex align-center gap-10">
                            <div style="font-size: 20px;">${cat.icon}</div>
                            <div>
                                <div>${cat.name}</div>
                                <div class="text-muted">Budget: ${formatCurrency(amount, 'AED')}</div>
                            </div>
                        </div>
                        <div class="text-right">
                            <div>${formatCurrency(spent, 'AED')}</div>
                            <div class="text-muted">${percentage.toFixed(0)}% used</div>
                        </div>
                    </div>
                `;
            }).join('');
        }

        // ========== BUDGET MANAGEMENT ==========
        function updateBudgetSpending(categoryId, amount) {
            const budget = budgets.find(b => b.categoryId === categoryId);
            if (budget) {
                budget.spent = (budget.spent || 0) + amount;
                saveAllData();
            }
        }

        function showBudgetModal() {
            const container = document.getElementById('budgetEditList');
            container.innerHTML = '';
            
            categories.forEach(category => {
                const budget = budgets.find(b => b.categoryId === category.id) || { amount: category.budget || 500 };
                
                container.innerHTML += `
                    <div class="form-group">
                        <label class="form-label">
                            <span style="font-size: 18px;">${category.icon}</span> 
                            ${category.name}
                        </label>
                        <div class="d-flex gap-10">
                            <input type="number" 
                                   class="form-input" 
                                   id="budget_${category.id}"
                                   value="${budget.amount}"
                                   placeholder="Monthly budget"
                                   step="0.01">
                            <span style="padding: 12px; color: var(--primary);">AED</span>
                        </div>
                    </div>
                `;
            });
            
            openModal('budgetModal');
        }

        function saveAllBudgets() {
            let hasChanges = false;
            
            categories.forEach(category => {
                const input = document.getElementById(`budget_${category.id}`);
                const newAmount = parseFloat(input.value) || 0;
                
                const existingBudgetIndex = budgets.findIndex(b => b.categoryId === category.id);
                
                if (existingBudgetIndex > -1) {
                    if (budgets[existingBudgetIndex].amount !== newAmount) {
                        budgets[existingBudgetIndex].amount = newAmount;
                        hasChanges = true;
                    }
                } else {
                    budgets.push({
                        id: Date.now() + Math.random(),
                        categoryId: category.id,
                        categoryName: category.name,
                        amount: newAmount,
                        period: 'monthly',
                        spent: 0,
                        createdAt: new Date().toISOString()
                    });
                    hasChanges = true;
                }
            });
            
            if (hasChanges) {
                saveAllData();
                updateAllDisplays();
                showNotification('Budgets updated');
            }
            
            closeModal('budgetModal');
        }

        function updateBudgetsList() {
            const container = document.getElementById('budgetsList');
            if (!container) return;
            
            if (budgets.length === 0) {
                container.innerHTML = `
                    <div class="loading">
                        <i class="fas fa-pie-chart"></i>
                        <div class="text-muted mt-10">No budgets set yet</div>
                        <button class="btn btn-primary mt-15" onclick="showBudgetModal()">
                            Set Budgets
                        </button>
                    </div>
                `;
                return;
            }
            
            container.innerHTML = budgets.map(budget => {
                const category = categories.find(c => c.id === budget.categoryId) || {};
                const spent = budget.spent || 0;
                const percentage = Math.min((spent / budget.amount) * 100, 100);
                const remaining = budget.amount - spent;
                
                let statusClass = '';
                let statusText = '';
                
                if (spent > budget.amount) {
                    statusClass = 'budget-warning';
                    statusText = `(${(spent - budget.amount).toFixed(0)} AED over)`;
                } else if (spent > budget.amount * 0.8) {
                    statusClass = 'budget-close';
                    statusText = 'Close to limit';
                }
                
                return `
                    <div class="budget-card" style="border-left-color: ${category.color || '#D4AF37'}">
                        <div class="budget-header">
                            <div class="budget-name">
                                ${category.icon || '📊'} ${budget.categoryName}
                            </div>
                            <div class="budget-amount ${statusClass}">
                                ${formatCurrency(spent, 'AED')} / ${formatCurrency(budget.amount, 'AED')}
                                ${statusText ? `<div class="text-muted">${statusText}</div>` : ''}
                            </div>
                        </div>
                        <div class="budget-progress">
                            <div class="budget-progress-bar" style="width: ${percentage}%; background: ${category.color || '#D4AF37'}"></div>
                        </div>
                        <div class="budget-stats">
                            <span>${percentage.toFixed(0)}% used</span>
                            <span>${formatCurrency(remaining, 'AED')} left</span>
                        </div>
                    </div>
                `;
            }).join('');
        }

        function updateBudgetOverview() {
            const container = document.getElementById('budgetOverview');
            if (!container) return;
            
            // Show only budgets with activity or close to limit
            const activeBudgets = budgets.filter(b => {
                const spent = b.spent || 0;
                return spent > 0 || (b.amount - spent) < 500;
            }).slice(0, 5);
            
            if (activeBudgets.length === 0) {
                container.innerHTML = '<div class="text-muted">No active budgets</div>';
                return;
            }
            
            container.innerHTML = activeBudgets.map(budget => {
                const category = categories.find(c => c.id === budget.categoryId) || {};
                const spent = budget.spent || 0;
                const remaining = budget.amount - spent;
                const percentage = Math.min((spent / budget.amount) * 100, 100);
                
                let statusClass = '';
                if (spent > budget.amount) {
                    statusClass = 'budget-warning';
                } else if (spent > budget.amount * 0.8) {
                    statusClass = 'budget-close';
                }
                
                return `
                    <div class="d-flex justify-between align-center mb-10">
                        <div>
                            <div class="stat-label">${category.icon || '📊'} ${budget.categoryName}</div>
                            <div class="stat-value ${statusClass}">
                                ${formatCurrency(spent, 'AED')} / ${formatCurrency(budget.amount, 'AED')}
                            </div>
                        </div>
                        <div class="text-right">
                            <div class="stat-label">Remaining</div>
                            <div class="stat-value">${formatCurrency(remaining, 'AED')}</div>
                        </div>
                    </div>
                `;
            }).join('');
        }

        // ========== TODO LIST MANAGEMENT ==========
        function showTodoModal() {
            const categorySelect = document.getElementById('todoCategory');
            categorySelect.innerHTML = '<option value="">Select category</option>';
            
            categories.forEach(cat => {
                const option = document.createElement('option');
                option.value = cat.id;
                option.textContent = `${cat.icon} ${cat.name}`;
                categorySelect.appendChild(option);
            });
            
            openModal('todoModal');
        }

        function saveTodoItem() {
            const nameInput = document.getElementById('todoName');
            const categorySelect = document.getElementById('todoCategory');
            const costInput = document.getElementById('todoCost');
            const profileSelect = document.getElementById('todoProfile');
            const prioritySelect = document.getElementById('todoPriority');
            
            const name = nameInput.value.trim();
            const categoryId = categorySelect.value;
            const cost = parseFloat(costInput.value) || 0;
            const profile = profileSelect.value;
            const priority = prioritySelect.value;
            
            if (!name) {
                showNotification('Please enter item name', 'error');
                return;
            }
            
            if (!categoryId) {
                showNotification('Please select a category', 'error');
                return;
            }
            
            const category = categories.find(c => c.id === categoryId);
            
            const todo = {
                id: Date.now(),
                name: name,
                categoryId: categoryId,
                categoryName: category.name,
                categoryIcon: category.icon,
                cost: cost,
                profile: profile,
                priority: priority,
                date: new Date().toISOString().split('T')[0],
                completed: false
            };
            
            todoItems.unshift(todo);
            saveAllData();
            updateTodoList();
            updateTodoStats();
            
            // Clear form
            nameInput.value = '';
            categorySelect.selectedIndex = 0;
            costInput.value = '';
            profileSelect.selectedIndex = 0;
            prioritySelect.selectedIndex = 0;
            
            closeModal('todoModal');
            showNotification('Item added to To-Buy list for ' + PROFILES[profile].name);
        }

        function updateTodoList() {
            const container = document.getElementById('todoList');
            if (!container) return;
            
            if (todoItems.length === 0) {
                container.innerHTML = `
                    <div class="loading">
                        <i class="fas fa-list-check"></i>
                        <div class="text-muted mt-10">No items in your to-buy list</div>
                    </div>
                `;
                return;
            }
            
            container.innerHTML = todoItems.map(item => {
                const category = categories.find(c => c.id === item.categoryId) || {};
                const priorityClass = `badge-${item.priority}`;
                
                return `
                    <div class="todo-item">
                        <div class="todo-content">
                            <div class="expense-title">${item.name}</div>
                            <div class="expense-meta">
                                <span>${formatCurrency(item.cost, 'AED')}</span>
                                <span>•</span>
                                <span>${category.icon || ''} ${category.name}</span>
                                <span>•</span>
                                <span class="user-badge ${item.profile}">${item.profile === 'malek' ? '👨' : '👩'} ${item.profile}</span>
                                <span>•</span>
                                <span class="badge ${priorityClass}">${item.priority}</span>
                            </div>
                        </div>
                        <div class="todo-actions">
                            <button class="btn btn-primary btn-sm" onclick="moveTodoToExpenses(${item.id})" title="Move to Expenses">
                                <i class="fas fa-receipt"></i> Expense
                            </button>
                            <button class="btn btn-danger btn-sm" onclick="deleteTodoItem(${item.id})">
                                <i class="fas fa-trash"></i>
                            </button>
                        </div>
                    </div>
                `;
            }).join('');
        }

        function updateTodoStats() {
            const totalItems = todoItems.length;
            const completedItems = todoItems.filter(item => item.completed).length;
            const totalCost = todoItems.reduce((sum, item) => sum + item.cost, 0);
            const completionRate = totalItems > 0 ? Math.round((completedItems / totalItems) * 100) : 0;
            
            document.getElementById('todoTotalCost').textContent = formatCurrency(totalCost, 'AED');
            document.getElementById('todoItemCount').textContent = totalItems;
            document.getElementById('todoCompleted').textContent = `${completionRate}%`;
        }

        function moveTodoToExpenses(todoId) {
            const todo = todoItems.find(t => t.id === todoId);
            if (!todo) return;
            
            // Create expense from todo
            const now = new Date();
            const expense = {
                id: Date.now(),
                amount: todo.cost,
                currency: 'AED',
                description: todo.name,
                categoryId: todo.categoryId,
                categoryName: todo.categoryName,
                categoryIcon: todo.categoryIcon,
                categoryColor: categories.find(c => c.id === todo.categoryId)?.color || '#D4AF37',
                profile: todo.profile,
                date: now.toISOString().split('T')[0],
                time: now.toLocaleTimeString([], { hour: '2-digit', minute: '2-digit' }),
                timestamp: now.getTime(),
                hasReceipt: false,
                fromTodo: true
            };
            
            expenses.unshift(expense);
            filteredExpenses.unshift(expense);
            
            // Update profile balance
            PROFILES[todo.profile].balance -= todo.cost;
            saveProfileBalances();
            
            // Remove from todo list
            todoItems = todoItems.filter(t => t.id !== todoId);
            
            // Update budget
            updateBudgetSpending(todo.categoryId, todo.cost);
            
            saveAllData();
            updateAllDisplays();
            filterExpenses();
            updateTodoStats();
            
            showNotification(`Moved "${todo.name}" to expenses for ${PROFILES[todo.profile].name}`);
        }

        function deleteTodoItem(todoId) {
            todoItems = todoItems.filter(t => t.id !== todoId);
            saveAllData();
            updateTodoList();
            updateTodoStats();
            showNotification('Item deleted');
        }

        // ========== GOALS MANAGEMENT ==========
        function showGoalModal() {
            openModal('goalModal');
        }

        function saveGoal() {
            const titleInput = document.getElementById('goalTitle');
            const targetInput = document.getElementById('goalTarget');
            const currentInput = document.getElementById('goalCurrent');
            const dateInput = document.getElementById('goalDate');
            const profileSelect = document.getElementById('goalProfile');
            const prioritySelect = document.getElementById('goalPriority');
            const descriptionInput = document.getElementById('goalDescription');
            
            const title = titleInput.value.trim();
            const target = parseFloat(targetInput.value) || 0;
            const current = parseFloat(currentInput.value) || 0;
            const targetDate = dateInput.value;
            const profile = profileSelect.value;
            const priority = prioritySelect.value;
            const description = descriptionInput.value.trim();
            
            if (!title) {
                showNotification('Please enter goal title', 'error');
                return;
            }
            
            if (target <= 0) {
                showNotification('Please enter a valid target amount', 'error');
                return;
            }
            
            const goal = {
                id: Date.now(),
                title: title,
                target: target,
                current: current,
                targetDate: targetDate,
                profile: profile,
                priority: priority,
                description: description,
                createdAt: new Date().toISOString(),
                completed: current >= target
            };
            
            goals.unshift(goal);
            saveAllData();
            updateGoalsList();
            
            // Clear form
            titleInput.value = '';
            targetInput.value = '';
            currentInput.value = '';
            dateInput.value = '';
            profileSelect.selectedIndex = 0;
            prioritySelect.selectedIndex = 0;
            descriptionInput.value = '';
            
            closeModal('goalModal');
            showNotification('Goal added successfully');
        }

        function updateGoalsList() {
            const container = document.getElementById('goalsList');
            if (!container) return;
            
            if (goals.length === 0) {
                container.innerHTML = `
                    <div style="text-align: center; padding: 40px; color: var(--text-light);">
                        <i class="fas fa-bullseye" style="font-size: 48px; margin-bottom: 20px; color: var(--primary);"></i>
                        <div>No goals set yet</div>
                        <button class="btn btn-primary mt-15" onclick="showGoalModal()">
                            Create Your First Goal
                        </button>
                    </div>
                `;
                return;
            }
            
            container.innerHTML = goals.map(goal => {
                const progress = goal.target > 0 ? (goal.current / goal.target) * 100 : 0;
                const daysLeft = goal.targetDate ? 
                    Math.ceil((new Date(goal.targetDate) - new Date()) / (1000 * 60 * 60 * 24)) : 
                    null;
                const priorityClass = `priority-${goal.priority}`;
                
                let statusText = '';
                if (goal.completed) {
                    statusText = `<span class="text-success">✓ Achieved!</span>`;
                } else if (daysLeft !== null) {
                    if (daysLeft < 0) {
                        statusText = `<span class="text-danger">Overdue</span>`;
                    } else if (daysLeft < 7) {
                        statusText = `<span class="text-warning">${daysLeft} days left</span>`;
                    } else {
                        statusText = `<span class="text-muted">${daysLeft} days left</span>`;
                    }
                }
                
                return `
                    <div class="goal-card">
                        <div class="goal-header">
                            <div class="goal-title">${goal.title}</div>
                            <div class="goal-priority ${priorityClass}">${goal.priority}</div>
                        </div>
                        
                        ${goal.description ? `
                            <div class="goal-details">${goal.description}</div>
                        ` : ''}
                        
                        <div class="goal-progress">
                            <div class="progress-bar">
                                <div class="progress-fill" style="width: ${Math.min(progress, 100)}%"></div>
                            </div>
                            <div class="progress-stats">
                                <span>${formatCurrency(goal.current, 'AED')} / ${formatCurrency(goal.target, 'AED')}</span>
                                <span>${progress.toFixed(1)}%</span>
                            </div>
                        </div>
                        
                        <div class="d-flex justify-between align-center">
                            <div>
                                ${statusText}
                                ${goal.targetDate ? `<div class="text-muted">Target: ${new Date(goal.targetDate).toLocaleDateString()}</div>` : ''}
                                ${goal.profile !== 'both' ? `<div class="text-muted">For: ${goal.profile}</div>` : ''}
                            </div>
                            <div class="goal-actions">
                                <button class="btn btn-danger btn-sm" onclick="deleteGoal(${goal.id})">
                                    <i class="fas fa-trash"></i>
                                </button>
                            </div>
                        </div>
                    </div>
                `;
            }).join('');
        }

        function deleteGoal(goalId) {
            if (confirm('Delete this goal?')) {
                goals = goals.filter(g => g.id !== goalId);
                saveAllData();
                updateGoalsList();
                showNotification('Goal deleted');
            }
        }

        // ========== EXPORT/IMPORT FUNCTIONS ==========
        function exportAllData() {
            const allData = {
                expenses: expenses,
                budgets: budgets,
                categories: categories,
                todoItems: todoItems,
                goals: goals,
                profileBalances: {
                    malek: PROFILES.malek.balance,
                    sabrina: PROFILES.sabrina.balance
                },
                exportDate: new Date().toISOString()
            };
            
            const dataStr = JSON.stringify(allData, null, 2);
            const dataBlob = new Blob([dataStr], { type: 'application/json' });
            const url = URL.createObjectURL(dataBlob);
            const link = document.createElement('a');
            link.href = url;
            link.download = `makkben-backup-${new Date().toISOString().split('T')[0]}.json`;
            link.click();
            
            showNotification('All data exported');
        }

        function createBackup() {
            exportAllData();
        }

        function restoreBackup(input) {
            const file = input.files[0];
            if (!file) return;
            
            const reader = new FileReader();
            reader.onload = function(e) {
                try {
                    const data = JSON.parse(e.target.result);
                    
                    if (data.expenses) expenses = data.expenses;
                    if (data.budgets) budgets = data.budgets;
                    if (data.categories) categories = data.categories;
                    if (data.todoItems) todoItems = data.todoItems;
                    if (data.goals) goals = data.goals;
                    if (data.profileBalances) {
                        PROFILES.malek.balance = data.profileBalances.malek || 5000;
                        PROFILES.sabrina.balance = data.profileBalances.sabrina || 5000;
                        document.getElementById('malekBalance').value = PROFILES.malek.balance;
                        document.getElementById('sabrinaBalance').value = PROFILES.sabrina.balance;
                        saveProfileBalances();
                    }
                    
                    filteredExpenses = [...expenses];
                    saveAllData();
                    initializeApp();
                    updateAllDisplays();
                    
                    showNotification('Backup restored successfully');
                } catch (error) {
                    showNotification('Error restoring backup', 'error');
                }
            };
            reader.readAsText(file);
        }

        function clearAllData() {
            if (confirm('Are you sure? This will delete ALL data except profile balances.')) {
                expenses = [];
                budgets = [];
                todoItems = [];
                categories = [...DEFAULT_CATEGORIES];
                goals = [];
                filteredExpenses = [];
                
                ensureAllCategoriesHaveBudgets();
                saveAllData();
                initializeApp();
                updateAllDisplays();
                
                showNotification('All data cleared');
            }
        }

        // ========== CALENDAR ==========
        function updateCalendar() {
            const monthNames = ['January', 'February', 'March', 'April', 'May', 'June',
                               'July', 'August', 'September', 'October', 'November', 'December'];
            
            document.getElementById('calendarMonth').textContent = 
                `${monthNames[currentMonth]} ${currentYear}`;
            
            const container = document.getElementById('calendarGrid');
            if (!container) return;
            
            const firstDay = new Date(currentYear, currentMonth, 1);
            const lastDay = new Date(currentYear, currentMonth + 1, 0);
            const daysInMonth = lastDay.getDate();
            
            const monthExpenses = expenses.filter(exp => {
                const expDate = new Date(exp.timestamp);
                return expDate.getMonth() === currentMonth && 
                       expDate.getFullYear() === currentYear;
            });
            
            const expensesByDay = {};
            monthExpenses.forEach(exp => {
                const day = new Date(exp.timestamp).getDate();
                if (!expensesByDay[day]) expensesByDay[day] = [];
                expensesByDay[day].push(exp);
            });
            
            container.innerHTML = '';
            
            for (let i = 0; i < firstDay.getDay(); i++) {
                const emptyElem = document.createElement('div');
                emptyElem.className = 'calendar-day';
                emptyElem.style.opacity = '0.3';
                container.appendChild(emptyElem);
            }
            
            const today = new Date();
            const isCurrentMonth = today.getMonth() === currentMonth && today.getFullYear() === currentYear;
            
            for (let day = 1; day <= daysInMonth; day++) {
                const dayElem = document.createElement('div');
                dayElem.className = 'calendar-day';
                dayElem.textContent = day;
                
                if (isCurrentMonth && day === today.getDate()) {
                    dayElem.classList.add('today');
                }
                
                if (expensesByDay[day]) {
                    dayElem.classList.add('has-expenses');
                    const total = expensesByDay[day].reduce((sum, exp) => 
                        sum + convertAmount(exp.amount, exp.currency, 'AED'), 0);
                    dayElem.title = `${total.toFixed(0)} AED spent`;
                    
                    const totalSpan = document.createElement('span');
                    totalSpan.className = 'day-expense-total';
                    totalSpan.textContent = `${total.toFixed(0)} AED`;
                    dayElem.appendChild(totalSpan);
                }
                
                container.appendChild(dayElem);
            }
        }

        function changeMonth(delta) {
            currentMonth += delta;
            
            if (currentMonth < 0) {
                currentMonth = 11;
                currentYear--;
            } else if (currentMonth > 11) {
                currentMonth = 0;
                currentYear++;
            }
            
            updateCalendar();
        }

        // ========== INITIAL SETUP ==========
        const isFirstRun = !localStorage.getItem('makkbenExpenses');
        if (isFirstRun) {
            ensureAllCategoriesHaveBudgets();
        }
    </script>
</body>
</html>
