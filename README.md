<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="اختبار الرخصة المهنية التفاعلي للمعلمين - إعداد المعلم فهد الخالدي">
<link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@300;400;500;700;800&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
<style>
:root {
    /* نظام ألوان متوهج ومشرق */
    --primary: #3B82F6;
    --primary-glow: #60A5FA;
    --primary-light: #93C5FD;
    
    --accent: #6366F1;
    --accent-glow: #8B5CF6;
    --accent-light: #A78BFA;
    
    --secondary: #10B981;
    --secondary-glow: #34D399;
    --secondary-light: #6EE7B7;
    
    --tertiary: #F59E0B;
    --tertiary-glow: #FBBF24;
    --tertiary-light: #FCD34D;
    
    --quaternary: #8B5CF6;
    --quaternary-glow: #A78BFA;
    --quaternary-light: #C4B5FD;
    
    --neon-blue: #00D4FF;
    --neon-purple: #A855F7;
    --neon-green: #00FF9D;
    --neon-yellow: #FFD700;
    --neon-pink: #FF0080;
    
    /* جرادينتز جديدة متوهجة */
    --primary-gradient: linear-gradient(135deg, var(--primary) 0%, var(--primary-glow) 50%, var(--primary-light) 100%);
    --accent-gradient: linear-gradient(135deg, var(--accent) 0%, var(--accent-glow) 50%, var(--neon-purple) 100%);
    --secondary-gradient: linear-gradient(135deg, var(--secondary) 0%, var(--secondary-glow) 50%, var(--neon-green) 100%);
    --tertiary-gradient: linear-gradient(135deg, var(--tertiary) 0%, var(--tertiary-glow) 50%, var(--neon-yellow) 100%);
    --neon-gradient: linear-gradient(135deg, var(--neon-blue) 0%, var(--neon-purple) 50%, var(--neon-pink) 100%);
    
    /* ظلال متوهجة */
    --glow-primary: 0 0 20px rgba(59, 130, 246, 0.7), 0 0 40px rgba(59, 130, 246, 0.5), 0 0 60px rgba(59, 130, 246, 0.3);
    --glow-accent: 0 0 20px rgba(99, 102, 241, 0.7), 0 0 40px rgba(99, 102, 241, 0.5), 0 0 60px rgba(99, 102, 241, 0.3);
    --glow-secondary: 0 0 20px rgba(16, 185, 129, 0.7), 0 0 40px rgba(16, 185, 129, 0.5), 0 0 60px rgba(16, 185, 129, 0.3);
    --glow-tertiary: 0 0 20px rgba(245, 158, 11, 0.7), 0 0 40px rgba(245, 158, 11, 0.5), 0 0 60px rgba(245, 158, 11, 0.3);
    --glow-neon: 0 0 20px rgba(0, 212, 255, 0.8), 0 0 40px rgba(168, 85, 247, 0.6), 0 0 60px rgba(255, 0, 128, 0.4);
    
    /* متغيرات التصميم */
    --bg: linear-gradient(135deg, var(--primary) 0%, var(--accent) 100%);
    --card-bg: rgba(255, 255, 255, 0.95);
    --text: #1F2937;
    --light-text: #6B7280;
    --border: rgba(59, 130, 246, 0.2);
    --shadow: 0 8px 32px rgba(59, 130, 246, 0.1);
    --shadow-hover: 0 20px 40px rgba(59, 130, 246, 0.2);
    --overlay-bg: rgba(0, 0, 0, 0.7);
}

.dark-theme {
    --bg: linear-gradient(135deg, #0F172A 0%, #1E293B 100%);
    --card-bg: rgba(30, 41, 59, 0.95);
    --text: #F1F5F9;
    --light-text: #CBD5E1;
    --border: rgba(59, 130, 246, 0.1);
    --shadow: 0 8px 32px rgba(0, 0, 0, 0.3);
    --shadow-hover: 0 20px 40px rgba(0, 0, 0, 0.4);
    --overlay-bg: rgba(0, 0, 0, 0.85);
}

* {
    box-sizing: border-box;
    font-family: 'Tajawal', Tahoma, Arial, sans-serif;
    margin: 0;
    padding: 0;
}

body {
    background: var(--bg);
    color: var(--text);
    line-height: 1.7;
    overflow-x: hidden;
    padding-top: 80px;
    transition: all 0.5s ease;
    min-height: 100vh;
}

/* Header بتصميم شفاف وجذاب */
header {
    background: rgba(59, 130, 246, 0.1);
    backdrop-filter: blur(20px);
    color: white;
    position: fixed;
    top: 0;
    width: 100%;
    z-index: 1000;
    box-shadow: var(--shadow);
    border-bottom: 1px solid var(--border);
    padding: 15px 0;
}

.header-container {
    max-width: 1200px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 20px;
}

.title-section h1 {
    font-size: 1.5rem;
    font-weight: 800;
    background: var(--accent-gradient);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    text-shadow: 0 2px 10px rgba(59, 130, 246, 0.3);
}

.header-actions {
    display: flex;
    gap: 10px;
}

.theme-btn, .back-btn, .whatsapp-btn {
    background: rgba(59, 130, 246, 0.2);
    color: white;
    border: 2px solid rgba(255, 255, 255, 0.3);
    padding: 10px 20px;
    border-radius: 15px;
    font-weight: 600;
    cursor: pointer;
    transition: all 0.3s ease;
    display: flex;
    align-items: center;
    gap: 8px;
    backdrop-filter: blur(20px);
    text-decoration: none;
    position: relative;
    overflow: hidden;
    box-shadow: 0 0 15px rgba(59, 130, 246, 0.3);
}

.theme-btn:hover, .back-btn:hover, .whatsapp-btn:hover {
    background: rgba(59, 130, 246, 0.3);
    transform: translateY(-3px);
    box-shadow: 0 0 25px rgba(59, 130, 246, 0.5), 0 5px 20px rgba(0, 0, 0, 0.2);
    border-color: rgba(255, 255, 255, 0.5);
}

/* تصميم زر الواتساب */
.whatsapp-btn {
    background: linear-gradient(135deg, #25D366 0%, #128C7E 100%);
    color: white;
    border: 2px solid rgba(255, 255, 255, 0.3);
    box-shadow: 0 0 20px rgba(37, 211, 102, 0.4);
    position: relative;
}

.whatsapp-btn:hover {
    background: linear-gradient(135deg, #128C7E 0%, #075E54 100%);
    transform: translateY(-3px);
    box-shadow: 0 0 30px rgba(37, 211, 102, 0.6);
    border-color: rgba(255, 255, 255, 0.5);
}

.whatsapp-btn i {
    font-size: 1.2em;
}

.btn-tooltip {
    position: absolute;
    bottom: -40px;
    right: 50%;
    transform: translateX(50%);
    background: rgba(0, 0, 0, 0.8);
    color: white;
    padding: 5px 10px;
    border-radius: 5px;
    font-size: 0.8rem;
    white-space: nowrap;
    opacity: 0;
    visibility: hidden;
    transition: all 0.3s ease;
    z-index: 1000;
    backdrop-filter: blur(10px);
}

.btn-tooltip::before {
    content: '';
    position: absolute;
    top: -5px;
    right: 50%;
    transform: translateX(50%);
    border-width: 0 5px 5px 5px;
    border-style: solid;
    border-color: transparent transparent rgba(0, 0, 0, 0.8) transparent;
}

.whatsapp-btn:hover .btn-tooltip {
    opacity: 1;
    visibility: visible;
    bottom: -35px;
}

/* Main Content */
main {
    max-width: 1000px;
    margin: 30px auto;
    padding: 0 20px;
}

/* تحديث الهيرو سكشن */
.hero-section {
    background: linear-gradient(135deg, rgba(59, 130, 246, 0.15), rgba(99, 102, 241, 0.15));
    backdrop-filter: blur(30px);
    color: white;
    border-radius: 24px;
    padding: 40px;
    margin-bottom: 30px;
    text-align: center;
    position: relative;
    overflow: hidden;
    box-shadow: 0 20px 60px rgba(59, 130, 246, 0.15),
                inset 0 1px 0 rgba(255, 255, 255, 0.2);
    border: 2px solid rgba(255, 255, 255, 0.1);
}

.hero-section::before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: var(--accent-gradient);
    opacity: 0.1;
    z-index: -1;
}

.hero-content {
    position: relative;
    z-index: 1;
}

.hero-title {
    font-size: 2.2rem;
    font-weight: 800;
    margin-bottom: 15px;
    background: linear-gradient(135deg, #fff 0%, #f0f0f0 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}

.hero-subtitle {
    font-size: 1.1rem;
    margin-bottom: 25px;
    opacity: 0.9;
    max-width: 600px;
    margin-left: auto;
    margin-right: auto;
}

/* Cards بتصميم زجاجي */
.card {
    background: rgba(255, 255, 255, 0.05);
    backdrop-filter: blur(30px);
    border-radius: 20px;
    padding: 30px;
    margin-bottom: 25px;
    box-shadow: 0 15px 35px rgba(0, 0, 0, 0.1),
                inset 0 1px 0 rgba(255, 255, 255, 0.1);
    transition: all 0.4s ease;
    border: 1px solid rgba(255, 255, 255, 0.1);
    position: relative;
    overflow: hidden;
}

.card::before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 5px;
    background: var(--neon-gradient);
}

.card:hover {
    transform: translateY(-8px) scale(1.02);
    box-shadow: var(--shadow-hover);
}

.section-title {
    text-align: center;
    color: var(--text);
    margin-bottom: 30px;
    font-size: 2rem;
    font-weight: 800;
    position: relative;
    padding-bottom: 15px;
}

.section-title::after {
    content: "";
    position: absolute;
    bottom: 0;
    right: 50%;
    transform: translateX(50%);
    width: 100px;
    height: 4px;
    background: var(--accent-gradient);
    border-radius: 2px;
}

/* تصميم الأسئلة */
.question-box {
    background: var(--card-bg);
    backdrop-filter: blur(20px);
    padding: 30px;
    margin-bottom: 25px;
    border-radius: 20px;
    box-shadow: var(--shadow);
    border: 1px solid var(--border);
    transition: all 0.4s ease;
    position: relative;
    overflow: hidden;
}

.question-box::before {
    content: "";
    position: absolute;
    top: 0;
    right: 0;
    width: 100%;
    height: 5px;
    background: var(--primary-gradient);
}

.question-box:hover {
    transform: translateY(-5px);
    box-shadow: var(--shadow-hover);
}

.question-number {
    font-size: 1.3em;
    color: var(--primary);
    margin-bottom: 15px;
    font-weight: bold;
    display: flex;
    align-items: center;
    gap: 10px;
}

.question-number i {
    color: var(--accent);
    font-size: 1.2em;
}

.question-text {
    font-size: 1.2em;
    margin-bottom: 25px;
    line-height: 1.7;
    color: var(--text);
    font-weight: 500;
}

.options {
    position: relative;
}

.options label {
    display: flex;
    align-items: center;
    padding: 18px 20px;
    margin: 12px 0;
    border: 2px solid var(--border);
    border-radius: 15px;
    cursor: pointer;
    transition: all 0.3s ease;
    background: var(--card-bg);
    position: relative;
    overflow: hidden;
    font-weight: 500;
}

.options label::before {
    content: "";
    position: absolute;
    left: 0;
    top: 0;
    height: 100%;
    width: 0;
    background: var(--primary-gradient);
    transition: width 0.3s ease;
    z-index: 0;
}

.options label:hover:not(.locked) {
    border-color: var(--primary);
    transform: translateX(-8px);
    box-shadow: 0 5px 15px rgba(59, 130, 246, 0.2);
}

.options label:hover:not(.locked)::before {
    width: 4px;
}

.options input[type="radio"] {
    margin-left: 12px;
    transform: scale(1.3);
    z-index: 1;
}

/* عندما تكون الإجابة مقفولة */
.options label.locked {
    cursor: not-allowed;
    opacity: 0.8;
    pointer-events: none;
}

.options input[type="radio"]:disabled {
    cursor: not-allowed;
}

.options label.selected {
    background: linear-gradient(135deg, rgba(59, 130, 246, 0.15), rgba(139, 92, 246, 0.15));
    border: 2px solid var(--accent);
    box-shadow: 0 0 15px rgba(99, 102, 241, 0.3);
}

.options label.selected::before {
    width: 6px;
    background: var(--success-gradient);
}

.options label.correct-answer {
    background: linear-gradient(135deg, rgba(16, 185, 129, 0.2), rgba(52, 211, 153, 0.2));
    border: 2px solid var(--secondary);
    box-shadow: 0 0 15px rgba(16, 185, 129, 0.3);
}

.options label.correct-answer::before {
    width: 6px;
    background: var(--secondary-gradient);
}

.options label.wrong-answer {
    background: linear-gradient(135deg, rgba(99, 102, 241, 0.2), rgba(139, 92, 246, 0.2));
    border: 2px solid var(--accent);
    box-shadow: 0 0 15px rgba(99, 102, 241, 0.3);
}

.options label.wrong-answer::before {
    width: 6px;
    background: var(--accent-gradient);
}

.correct {
    color: var(--secondary);
    font-weight: bold;
}

.wrong {
    color: var(--accent);
    font-weight: bold;
}

.explanation {
    margin-top: 25px;
    padding: 25px;
    border-radius: 15px;
    display: none;
    background: linear-gradient(135deg, rgba(59, 130, 246, 0.05), rgba(99, 102, 241, 0.05));
    border-left: 4px solid var(--secondary);
    animation: slideDown 0.5s ease;
    backdrop-filter: blur(10px);
}

@keyframes slideDown {
    from {
        opacity: 0;
        transform: translateY(-15px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

.explanation-line {
    padding: 15px;
    margin: 10px 0;
    border-radius: 10px;
    transition: all 0.3s ease;
}

.explanation-correct {
    background: linear-gradient(135deg, rgba(16, 185, 129, 0.1), rgba(52, 211, 153, 0.1));
    border-right: 3px solid var(--secondary);
}

.explanation-wrong-1 {
    background: linear-gradient(135deg, rgba(99, 102, 241, 0.1), rgba(139, 92, 246, 0.1));
    border-right: 3px solid var(--accent);
}

.explanation-wrong-2 {
    background: linear-gradient(135deg, rgba(245, 158, 11, 0.1), rgba(251, 191, 36, 0.1));
    border-right: 3px solid var(--tertiary);
}

.explanation-wrong-3 {
    background: linear-gradient(135deg, rgba(139, 92, 246, 0.1), rgba(196, 181, 253, 0.1));
    border-right: 3px solid var(--quaternary);
}

/* تحديث تصميم الأزرار الرئيسية */
.btn-primary {
    background: var(--accent-gradient);
    color: white;
    box-shadow: var(--glow-accent), 0 8px 25px rgba(99, 102, 241, 0.4);
    border: 2px solid rgba(255, 255, 255, 0.3);
    position: relative;
    overflow: hidden;
    z-index: 1;
    transition: all 0.4s ease;
}

.btn-primary::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.4), transparent);
    transition: left 0.7s;
    z-index: -1;
}

.btn-primary:hover {
    transform: translateY(-8px) scale(1.05);
    box-shadow: var(--glow-accent), 0 15px 40px rgba(99, 102, 241, 0.6);
    border-color: rgba(255, 255, 255, 0.5);
}

.btn-primary:hover::before {
    left: 100%;
}

.btn-primary:active {
    transform: translateY(-4px) scale(1.02);
}

.btn-secondary {
    background: var(--primary-gradient);
    color: white;
    box-shadow: var(--glow-primary), 0 8px 25px rgba(59, 130, 246, 0.4);
    border: 2px solid rgba(255, 255, 255, 0.3);
    position: relative;
    overflow: hidden;
    z-index: 1;
}

.btn-secondary::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.4), transparent);
    transition: left 0.7s;
    z-index: -1;
}

.btn-secondary:hover {
    transform: translateY(-8px) scale(1.05);
    box-shadow: var(--glow-primary), 0 15px 40px rgba(59, 130, 246, 0.6);
    border-color: rgba(255, 255, 255, 0.5);
}

.btn-secondary:hover::before {
    left: 100%;
}

/* أزرار خاصة إضافية */
.btn-neon {
    background: var(--neon-gradient);
    color: white;
    box-shadow: var(--glow-neon), 0 8px 25px rgba(0, 212, 255, 0.4);
    border: 2px solid rgba(255, 255, 255, 0.3);
    animation: neon-pulse 2s infinite alternate;
}

@keyframes neon-pulse {
    0% {
        box-shadow: var(--glow-neon), 0 8px 25px rgba(0, 212, 255, 0.4);
    }
    100% {
        box-shadow: 0 0 25px rgba(0, 212, 255, 0.8),
                    0 0 50px rgba(168, 85, 247, 0.6),
                    0 0 75px rgba(255, 0, 128, 0.4),
                    0 15px 40px rgba(0, 212, 255, 0.6);
    }
}

.btn-success {
    background: var(--secondary-gradient);
    color: white;
    box-shadow: var(--glow-secondary), 0 8px 25px rgba(16, 185, 129, 0.4);
    border: 2px solid rgba(255, 255, 255, 0.3);
}

.btn-warning {
    background: var(--tertiary-gradient);
    color: white;
    box-shadow: var(--glow-tertiary), 0 8px 25px rgba(245, 158, 11, 0.4);
    border: 2px solid rgba(255, 255, 255, 0.3);
}

/* Navigation Buttons */
.navigation {
    display: flex;
    justify-content: space-between;
    margin-top: 30px;
    gap: 20px;
}

.btn {
    padding: 15px 30px;
    border-radius: 15px;
    font-weight: 700;
    text-decoration: none;
    transition: all 0.3s ease;
    display: inline-flex;
    align-items: center;
    gap: 10px;
    font-size: 1rem;
    border: none;
    cursor: pointer;
    position: relative;
    overflow: hidden;
}

.btn::before {
    content: "";
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(255,255,255,0.3), transparent);
    transition: left 0.6s;
}

.btn:hover::before {
    left: 100%;
}

.btn:disabled {
    background: #9CA3AF;
    cursor: not-allowed;
    transform: none;
    box-shadow: none;
    opacity: 0.6;
}

.btn:disabled:hover::before {
    left: -100%;
}

/* Progress Bar */
.progress-bar {
    height: 15px;
    background: rgba(255, 255, 255, 0.2);
    border-radius: 10px;
    margin-bottom: 30px;
    overflow: hidden;
    box-shadow: inset 0 2px 5px rgba(0, 0, 0, 0.1);
    position: relative;
    backdrop-filter: blur(10px);
}

.progress {
    height: 100%;
    background: var(--neon-gradient);
    box-shadow: 0 0 15px rgba(0, 212, 255, 0.5);
    width: 0%;
    transition: width 0.5s ease;
    border-radius: 10px;
    position: relative;
    overflow: hidden;
}

.progress::after {
    content: "";
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(255,255,255,0.4), transparent);
    animation: shimmer 1.5s infinite;
}

@keyframes shimmer {
    0% { left: -100%; }
    100% { left: 100%; }
}

/* Results Box */
#result-box, #current-score {
    background: var(--card-bg);
    backdrop-filter: blur(20px);
    padding: 30px;
    margin-top: 30px;
    border-radius: 20px;
    box-shadow: var(--shadow);
    border: 1px solid var(--border);
    display: none;
    animation: slideUp 0.6s ease;
}

@keyframes slideUp {
    from {
        opacity: 0;
        transform: translateY(30px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

.controls {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 30px;
    flex-wrap: wrap;
    gap: 20px;
}

.quiz-info {
    font-size: 1rem;
    color: var(--light-text);
    background: linear-gradient(135deg, rgba(59, 130, 246, 0.1), rgba(99, 102, 241, 0.1));
    padding: 10px 20px;
    border-radius: 25px;
    font-weight: 600;
    backdrop-filter: blur(10px);
}

/* تحديث المؤقت */
#timer {
    font-size: 1.1rem;
    font-weight: bold;
    color: white;
    margin-left: 20px;
    display: flex;
    align-items: center;
    gap: 8px;
    background: rgba(0, 212, 255, 0.2);
    backdrop-filter: blur(20px);
    padding: 10px 20px;
    border-radius: 25px;
    border: 2px solid rgba(0, 212, 255, 0.3);
    box-shadow: 0 0 15px rgba(0, 212, 255, 0.2);
}

.timer-warning {
    background: rgba(255, 0, 128, 0.2) !important;
    border-color: rgba(255, 0, 128, 0.3) !important;
    box-shadow: 0 0 20px rgba(255, 0, 128, 0.3) !important;
    animation: warning-pulse 0.8s infinite alternate;
}

@keyframes warning-pulse {
    from {
        box-shadow: 0 0 15px rgba(255, 0, 128, 0.3);
    }
    to {
        box-shadow: 0 0 25px rgba(255, 0, 128, 0.5), 0 0 40px rgba(255, 0, 128, 0.3);
    }
}

@keyframes pulse {
    0% { transform: scale(1); }
    50% { transform: scale(1.05); }
    100% { transform: scale(1); }
}

/* تحسينات لقائمة الأسئلة - نافذة منبثقة في المنتصف */
.overlay {
    display: none;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: var(--overlay-bg);
    z-index: 2000;
    backdrop-filter: blur(10px);
    animation: fadeIn 0.3s ease;
}

.questions-modal {
    position: fixed;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 90%;
    max-width: 800px;
    max-height: 80vh;
    overflow-y: auto;
    background: var(--card-bg);
    backdrop-filter: blur(30px);
    border-radius: 24px;
    padding: 30px;
    box-shadow: 0 25px 50px rgba(0, 0, 0, 0.3);
    border: 1px solid var(--border);
    z-index: 2001;
    animation: modalSlideIn 0.4s ease;
}

@keyframes modalSlideIn {
    from {
        opacity: 0;
        transform: translate(-50%, -60%);
    }
    to {
        opacity: 1;
        transform: translate(-50%, -50%);
    }
}

@keyframes fadeIn {
    from {
        opacity: 0;
    }
    to {
        opacity: 1;
    }
}

.modal-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 25px;
    padding-bottom: 15px;
    border-bottom: 2px solid var(--border);
}

.modal-title {
    font-size: 1.5rem;
    font-weight: 700;
    color: var(--text);
    display: flex;
    align-items: center;
    gap: 10px;
}

.close-modal {
    background: var(--accent-gradient);
    color: white;
    border: none;
    width: 40px;
    height: 40px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    cursor: pointer;
    font-size: 1.2rem;
    transition: all 0.3s ease;
    box-shadow: var(--glow-accent);
}

.close-modal:hover {
    transform: rotate(90deg) scale(1.1);
}

#questions-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(60px, 1fr));
    gap: 12px;
    margin: 20px 0;
}

.question-status-grid {
    width: 60px;
    height: 60px;
    border: 2px solid rgba(59, 130, 246, 0.3);
    border-radius: 15px;
    display: flex;
    align-items: center;
    justify-content: center;
    cursor: pointer;
    font-weight: 700;
    transition: all 0.3s ease;
    background: var(--card-bg);
    position: relative;
    overflow: hidden;
    font-size: 1.1rem;
}

.question-status-grid::before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: var(--accent-gradient);
    opacity: 0;
    transition: opacity 0.3s ease;
}

.question-status-grid:hover:not(.locked) {
    transform: translateY(-3px) scale(1.1);
    box-shadow: var(--shadow);
}

.question-status-grid.current {
    background: var(--accent-gradient);
    border-color: rgba(255, 255, 255, 0.5);
    box-shadow: var(--glow-accent), 0 5px 15px rgba(99, 102, 241, 0.3);
    animation: pulse 2s infinite;
}

.question-status-grid.answered {
    background: var(--secondary-gradient);
    border-color: rgba(255, 255, 255, 0.5);
    box-shadow: var(--glow-secondary), 0 5px 15px rgba(16, 185, 129, 0.3);
}

.question-status-grid.flagged {
    background: var(--tertiary-gradient);
    border-color: rgba(255, 255, 255, 0.5);
    box-shadow: var(--glow-tertiary), 0 5px 15px rgba(245, 158, 11, 0.3);
}

.question-status-grid.locked {
    cursor: not-allowed;
    opacity: 0.7;
}

.question-status-grid span {
    position: relative;
    z-index: 1;
}

.legend {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    margin-top: 20px;
    font-size: 0.9rem;
}

.legend-item {
    display: flex;
    align-items: center;
    gap: 10px;
}

/* تحسينات للوضع الداكن */
.dark-theme {
    --bg: linear-gradient(135deg, #0F172A 0%, #1E293B 100%);
    --card-bg: rgba(30, 41, 59, 0.95);
    --text: #F1F5F9;
    --light-text: #CBD5E1;
    --border: rgba(59, 130, 246, 0.1);
    --shadow: 0 8px 32px rgba(0, 0, 0, 0.3);
    --shadow-hover: 0 20px 40px rgba(0, 0, 0, 0.4);
    --overlay-bg: rgba(0, 0, 0, 0.85);
}

.dark-theme .btn-primary,
.dark-theme .btn-secondary {
    border-color: rgba(255, 255, 255, 0.2);
}

.dark-theme .theme-btn,
.dark-theme .back-btn,
.dark-theme .whatsapp-btn {
    background: rgba(59, 130, 246, 0.15);
    border-color: rgba(255, 255, 255, 0.2);
}

.dark-theme .whatsapp-btn {
    background: linear-gradient(135deg, #075E54 0%, #128C7E 100%);
    border-color: rgba(255, 255, 255, 0.2);
}

.dark-theme .card {
    background: rgba(30, 41, 59, 0.7);
    border-color: rgba(255, 255, 255, 0.05);
}

.dark-theme .hero-section {
    background: linear-gradient(135deg, rgba(59, 130, 246, 0.1), rgba(99, 102, 241, 0.1));
    border-color: rgba(255, 255, 255, 0.05);
}

/* Responsive Design */
@media (max-width: 768px) {
    body {
        padding-top: 70px;
    }
    
    .header-container {
        padding: 0 15px;
        flex-direction: column;
        gap: 15px;
    }
    
    .title-section h1 {
        font-size: 1.3rem;
    }
    
    .hero-title {
        font-size: 1.8rem;
    }
    
    .hero-subtitle {
        font-size: 1rem;
    }
    
    .card, .question-box {
        padding: 25px;
    }
    
    .navigation {
        flex-direction: column;
        gap: 15px;
    }
    
    .btn {
        width: 100%;
        justify-content: center;
        padding: 14px 25px;
        font-size: 1rem;
    }
    
    .theme-btn, .back-btn, .whatsapp-btn {
        padding: 8px 15px;
        font-size: 0.9rem;
    }
    
    .controls {
        flex-direction: column;
        align-items: stretch;
    }
    
    .questions-modal {
        width: 95%;
        padding: 20px;
    }
    
    #questions-grid {
        grid-template-columns: repeat(auto-fill, minmax(50px, 1fr));
    }
    
    .question-status-grid {
        width: 50px;
        height: 50px;
        font-size: 1rem;
    }
    
    /* تحسين responsive design لزر الواتساب */
    .btn-tooltip {
        display: none;
    }
    
    .whatsapp-btn span:not(.btn-tooltip) {
        display: none;
    }
}

@media (max-width: 480px) {
    .header-container {
        text-align: center;
    }
    
    .header-actions {
        justify-content: center;
    }
    
    .question-box {
        padding: 20px;
    }
    
    .options label {
        padding: 15px;
    }
    
    .hero-section {
        padding: 25px;
    }
    
    .section-title {
        font-size: 1.6rem;
    }
    
    .questions-modal {
        padding: 15px;
    }
    
    #questions-grid {
        grid-template-columns: repeat(auto-fill, minmax(45px, 1fr));
        gap: 8px;
    }
    
    .question-status-grid {
        width: 45px;
        height: 45px;
        font-size: 0.9rem;
    }
}

/* تأثيرات إضافية */
.fade-in {
    animation: fadeIn 0.8s ease;
}

@keyframes fadeIn {
    from {
        opacity: 0;
        transform: translateY(20px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

.bounce-in {
    animation: bounceIn 0.8s ease;
}

@keyframes bounceIn {
    0% {
        opacity: 0;
        transform: scale(0.3);
    }
    50% {
        opacity: 1;
        transform: scale(1.05);
    }
    70% {
        transform: scale(0.95);
    }
    100% {
        opacity: 1;
        transform: scale(1);
    }
}

/* تأثيرات الجلاس مورفيزم */
.glass-effect {
    background: rgba(255, 255, 255, 0.1);
    backdrop-filter: blur(20px);
    border: 1px solid rgba(255, 255, 255, 0.2);
}

/* رسوم متحركة للخلفية */
.bg-animation {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: -1;
    opacity: 0.3;
}

.floating-shapes {
    position: absolute;
    width: 100%;
    height: 100%;
}

.shape {
    position: absolute;
    background: var(--neon-gradient);
    opacity: 0.08;
    filter: blur(40px);
    border-radius: 50%;
    animation: float 6s ease-in-out infinite;
}

.shape:nth-child(1) {
    width: 100px;
    height: 100px;
    top: 10%;
    left: 10%;
    animation-delay: 0s;
}

.shape:nth-child(2) {
    width: 150px;
    height: 150px;
    top: 60%;
    right: 10%;
    animation-delay: 2s;
}

.shape:nth-child(3) {
    width: 80px;
    height: 80px;
    bottom: 20%;
    left: 20%;
    animation-delay: 4s;
}

@keyframes float {
    0%, 100% {
        transform: translateY(0) rotate(0deg);
    }
    50% {
        transform: translateY(-20px) rotate(180deg);
    }
}

/* تأثيرات إضافية للتفاعل */
.btn:focus {
    outline: none;
    animation: button-focus 0.3s ease;
}

@keyframes button-focus {
    0% {
        transform: scale(1);
    }
    50% {
        transform: scale(1.05);
    }
    100% {
        transform: scale(1);
    }
}
</style>
</head>
<body>
<!-- رسوم متحركة للخلفية -->
<div class="bg-animation">
    <div class="floating-shapes">
        <div class="shape"></div>
        <div class="shape"></div>
        <div class="shape"></div>
    </div>
</div>

<!-- Header -->
<header class="glass-effect">
    <div class="header-container">
        <div class="title-section">
            <h1>اختبار الرخصة المهنية التفاعلي</h1>
        </div>
        <div class="header-actions">
            <button class="theme-btn" id="themeBtn">
                <i class="fas fa-moon"></i>
            </button>
            <button class="whatsapp-btn" id="whatsappBtn" title="الإبلاغ عن خطأ أو ملاحظة">
                <i class="fab fa-whatsapp"></i>
                <span class="btn-tooltip">الإبلاغ عن خطأ</span>
            </button>
            <a href="#" class="back-btn">
                <i class="fas fa-arrow-right"></i>
                العودة للرئيسية
            </a>
        </div>
    </div>
</header>

<!-- Main Content -->
<main>
    <!-- Hero Section -->
    <section class="hero-section glass-effect">
        <div class="hero-content">
            <h1 class="hero-title">اختبار الرخصة المهنية للمعلمين</h1>
            <p class="hero-subtitle">تم إعداد هذا الاختبار التفاعلي لمحاكاة الاختبار الرسمي للرخصة المهنية، ويقدم تغذية راجعة فورية لجميع الإجابات</p>
            <div class="quiz-info">إعداد: المعلم فهد الخالدي</div>
        </div>
    </section>

    <!-- Progress Bar -->
    <div class="progress-bar glass-effect">
        <div class="progress" id="progress"></div>
    </div>

    <!-- Quiz Container -->
    <div id="quiz"></div>

    <!-- Controls -->
    <div class="controls">
        <div class="quiz-info" id="quiz-info"></div>
        <div id="timer">⏱️ <span id="time-display">45:00</span></div>
        <div style="display: flex; gap: 15px; flex-wrap: wrap;">
            <button class="btn btn-primary" onclick="showQuestionsList()">
                <i class="fas fa-list"></i>
                قائمة الأسئلة
            </button>
            <button class="btn btn-warning" onclick="toggleMarkForReview()" id="mark-review-btn">
                <i class="fas fa-flag"></i>
                وضع علامة للمراجعة
            </button>
            <button class="btn btn-neon" onclick="finishQuiz()">
                <i class="fas fa-flag-checkered"></i>
                إنهاء الاختبار
            </button>
            <button class="btn btn-secondary" onclick="showCurrentScore()">
                <i class="fas fa-chart-bar"></i>
                عرض الدرجات الحالية
            </button>
        </div>
    </div>

    <!-- نافذة قائمة الأسئلة المنبثقة -->
    <div id="questions-overlay" class="overlay" onclick="hideQuestionsList()"></div>
    <div id="questions-modal" class="questions-modal">
        <div class="modal-header">
            <h3 class="modal-title">
                <i class="fas fa-th-list"></i>
                قائمة الأسئلة
            </h3>
            <button class="close-modal" onclick="hideQuestionsList()">
                <i class="fas fa-times"></i>
            </button>
        </div>
        <div id="questions-grid"></div>
        <div class="legend">
            <div class="legend-item">
                <div class="question-status-grid" style="background: var(--accent-gradient); color: white;"></div>
                <span>السؤال الحالي</span>
            </div>
            <div class="legend-item">
                <div class="question-status-grid" style="background: var(--secondary-gradient); color: white;"></div>
                <span>تمت الإجابة</span>
            </div>
            <div class="legend-item">
                <div class="question-status-grid" style="background: var(--tertiary-gradient); color: var(--text);"></div>
                <span>معلم للمراجعة</span>
            </div>
            <div class="legend-item">
                <div class="question-status-grid" style="background: var(--card-bg); border-color: var(--border);"></div>
                <span>لم يتم الإجابة</span>
            </div>
        </div>
        <button class="btn btn-primary" onclick="hideQuestionsList()" style="margin-top:20px; width: 100%;">
            <i class="fas fa-times"></i>
            إغلاق القائمة
        </button>
    </div>

    <!-- Current Score -->
    <div id="current-score" class="card">
        <h3 style="color: var(--text); margin-bottom: 20px; display: flex; align-items: center; gap: 12px;">
            <i class="fas fa-chart-bar"></i>
            الدرجات الحالية
        </h3>
        <p id="current-correct" style="margin-bottom: 15px; font-size: 1.1rem;"></p>
        <p id="current-percentage" style="font-weight: bold; font-size: 1.3rem; color: var(--primary);"></p>
    </div>

    <!-- Final Results -->
    <div id="result-box" class="card">
        <h3 id="result" style="color: var(--text); margin-bottom: 20px;"></h3>
        <p id="percentage" style="font-size: 1.4rem; margin-bottom: 15px;"></p>
        <p id="evaluation" style="font-weight: bold; font-size: 1.3rem;"></p>
    </div>
</main>

<script>
// مصفوفة فارغة من الأسئلة
const questions = [];

let currentQuestionIndex = 0;
let userAnswers = Array(questions.length).fill(null);
let timeLeft = 45 * 60; // 45 دقيقة
let timerInterval;
let markedQuestions = [];
let answerLocked = Array(questions.length).fill(false);

// زر الواتساب للإبلاغ عن الأخطاء
document.getElementById('whatsappBtn').addEventListener('click', function() {
    // رسالة جاهزة للإبلاغ
    const currentQuestion = currentQuestionIndex + 1;
    const message = `السلام عليكم ورحمة الله وبركاته

أود الإبلاغ عن ملاحظة في اختبار الرخصة المهنية:

• السؤال رقم: ${currentQuestion}
• الملاحظة: [يرجى كتابة الملاحظة هنا]

مع الشكر والتقدير`;

    // رقم الواتساب
    const phoneNumber = '966597077245';
    // رابط واتساب مع الرسالة الجاهزة
    const whatsappUrl = `https://wa.me/${phoneNumber}?text=${encodeURIComponent(message)}`;
    // فتح الواتساب في نافذة جديدة
    window.open(whatsappUrl, '_blank');
});

// تحديث زر الواتساب مع الوضع الداكن
function updateWhatsappButton() {
    const whatsappBtn = document.getElementById('whatsappBtn');
    if (document.body.classList.contains('dark-theme')) {
        whatsappBtn.style.background = 'linear-gradient(135deg, #075E54 0%, #128C7E 100%)';
        whatsappBtn.style.borderColor = 'rgba(255, 255, 255, 0.2)';
    } else {
        whatsappBtn.style.background = 'linear-gradient(135deg, #25D366 0%, #128C7E 100%)';
        whatsappBtn.style.borderColor = 'rgba(255, 255, 255, 0.3)';
    }
}

// التحقق من تفضيل الوضع الداكن المخزن
function checkDarkModePreference() {
    const darkMode = localStorage.getItem('darkMode');
    const themeBtn = document.getElementById('themeBtn');
    const icon = themeBtn.querySelector('i');
    
    if (darkMode === 'enabled') {
        document.body.classList.add('dark-theme');
        icon.classList.remove('fa-moon');
        icon.classList.add('fa-sun');
    } else {
        document.body.classList.remove('dark-theme');
        icon.classList.remove('fa-sun');
        icon.classList.add('fa-moon');
    }
    updateWhatsappButton();
}

// تبديل الوضع الليلي/النهاري
document.getElementById('themeBtn').addEventListener('click', function() {
    document.body.classList.toggle('dark-theme');
    const icon = this.querySelector('i');
    
    if (document.body.classList.contains('dark-theme')) {
        icon.classList.remove('fa-moon');
        icon.classList.add('fa-sun');
        localStorage.setItem('darkMode', 'enabled');
    } else {
        icon.classList.remove('fa-sun');
        icon.classList.add('fa-moon');
        localStorage.setItem('darkMode', 'disabled');
    }
    updateWhatsappButton();
});

// المؤقت
function startTimer() {
    timerInterval = setInterval(() => {
        timeLeft--;
        updateTimerDisplay();
        
        if (timeLeft <= 0) {
            clearInterval(timerInterval);
            finishQuiz();
        }
    }, 1000);
}

function updateTimerDisplay() {
    const minutes = Math.floor(timeLeft / 60);
    const seconds = timeLeft % 60;
    const timeDisplay = document.getElementById('time-display');
    timeDisplay.textContent = `${minutes.toString().padStart(2, '0')}:${seconds.toString().padStart(2, '0')}`;
    
    if (timeLeft < 300) { // 5 دقائق
        timeDisplay.classList.add('timer-warning');
    } else {
        timeDisplay.classList.remove('timer-warning');
    }
}

// عرض قائمة الأسئلة كنافذة منبثقة
function showQuestionsList() {
    const grid = document.getElementById('questions-grid');
    grid.innerHTML = '';
    
    questions.forEach((_, index) => {
        const btn = document.createElement('div');
        btn.className = `question-status-grid ${index === currentQuestionIndex ? 'current' : ''} ${userAnswers[index] !== null ? 'answered' : ''} ${markedQuestions.includes(index) ? 'flagged' : ''}`;
        btn.innerHTML = `<span>${index + 1}</span>`;
        btn.onclick = () => {
            currentQuestionIndex = index;
            loadQuiz();
            hideQuestionsList();
        };
        grid.appendChild(btn);
    });
    
    document.getElementById('questions-overlay').style.display = 'block';
    document.getElementById('questions-modal').style.display = 'block';
    document.body.style.overflow = 'hidden'; // منع التمرير عند فتح النافذة
}

function hideQuestionsList() {
    document.getElementById('questions-overlay').style.display = 'none';
    document.getElementById('questions-modal').style.display = 'none';
    document.body.style.overflow = 'auto'; // إعادة التمرير
}

// وضع علامة للمراجعة
function toggleMarkForReview() {
    const index = markedQuestions.indexOf(currentQuestionIndex);
    const btn = document.getElementById('mark-review-btn');
    
    if (index === -1) {
        markedQuestions.push(currentQuestionIndex);
        btn.innerHTML = '<i class="fas fa-flag"></i> إزالة العلامة';
        btn.style.background = 'var(--tertiary-gradient)';
    } else {
        markedQuestions.splice(index, 1);
        btn.innerHTML = '<i class="fas fa-flag"></i> وضع علامة للمراجعة';
        btn.style.background = 'var(--secondary-gradient)';
    }
    
    if (document.getElementById('questions-overlay').style.display === 'block') {
        showQuestionsList();
    }
}

// تحميل الاختبار
function loadQuiz() {
    const quizDiv = document.getElementById("quiz");
    
    if (questions.length === 0) {
        quizDiv.innerHTML = `
            <div class="card fade-in">
                <h3 style="color: var(--text); margin-bottom: 20px; text-align: center;">
                    <i class="fas fa-info-circle" style="color: var(--primary); margin-left: 10px;"></i>68 سؤال مع تغذية راجعة فورية
                </h3>
                <p style="text-align: center; color: var(--light-text); margin-bottom: 20px;">
                    تم جمع الاسئلة من خلال تجمعيات الأعوام السابقة .
                </p>
                <div style="text-align: center;">
                    <button class="btn btn-neon" onclick="addSampleQuestions()">
                        <i class="fas fa-plus"></i>
                        إبدأ الاختبار
                    </button>
                </div>
            </div>
        `;
        return;
    }
    
    const question = questions[currentQuestionIndex];
    const isLocked = answerLocked[currentQuestionIndex];
    
    let html = `
        <div class="question-box fade-in">
            <div class="question-number">
                <i class="fas fa-question-circle"></i>
                السؤال ${currentQuestionIndex + 1} من ${questions.length}
                ${isLocked ? '<span style="color: var(--accent); margin-right: 10px;"><i class="fas fa-lock"></i> مقفل</span>' : ''}
            </div>
            <div class="question-text">${question.q}</div>
            <div class="options">
    `;
    
    question.options.forEach((opt, i) => {
        const isChecked = userAnswers[currentQuestionIndex] === i;
        const isDisabled = isLocked;
        let labelClass = '';
        
        if (isLocked) {
            labelClass = 'locked';
            if (isChecked) {
                labelClass += userAnswers[currentQuestionIndex] === question.answer ? ' correct-answer' : ' wrong-answer';
            } else if (i === question.answer) {
                labelClass += ' correct-answer';
            }
        } else if (isChecked) {
            labelClass = 'selected';
        }
        
        html += `
            <label class="${labelClass}">
                <input type="radio" name="q${currentQuestionIndex}" value="${i}" ${isChecked ? 'checked' : ''} ${isDisabled ? 'disabled' : ''} onchange="selectAnswer(${i})" ${isLocked ? 'onclick="return false;"' : ''}>
                ${opt}
                ${isLocked && i === question.answer ? ' <i class="fas fa-check" style="color: var(--secondary); margin-right: 5px;"></i>' : ''}
            </label>
        `;
    });
    
    html += `
            </div>
            <div id="explanation" class="explanation"></div>
        </div>
        <div class="navigation">
            <button class="btn btn-secondary" onclick="previousQuestion()" ${currentQuestionIndex === 0 ? 'disabled' : ''}>
                <i class="fas fa-arrow-right"></i>
                السابق
            </button>
            <button class="btn btn-primary" onclick="nextQuestion()" ${currentQuestionIndex === questions.length - 1 ? 'disabled' : ''}>
                التالي
                <i class="fas fa-arrow-left"></i>
            </button>
        </div>
    `;
    
    quizDiv.innerHTML = html;
    
    // تحديث شريط التقدم
    document.getElementById('progress').style.width = questions.length > 0 ? `${((currentQuestionIndex + 1) / questions.length) * 100}%` : '0%';
    
    // تحديث معلومات الاختبار
    document.getElementById('quiz-info').innerHTML = questions.length > 0 ? `السؤال ${currentQuestionIndex + 1} من ${questions.length}` : 'لا توجد أسئلة';
    
    // تحديث زر وضع العلامة
    const markBtn = document.getElementById('mark-review-btn');
    if (markedQuestions.includes(currentQuestionIndex)) {
        markBtn.innerHTML = '<i class="fas fa-flag"></i> إزالة العلامة';
        markBtn.style.background = 'var(--tertiary-gradient)';
    } else {
        markBtn.innerHTML = '<i class="fas fa-flag"></i> وضع علامة للمراجعة';
        markBtn.style.background = 'var(--secondary-gradient)';
    }
    // عرض الشرح إذا كان المستخدم قد أجاب على السؤال
    if (userAnswers[currentQuestionIndex] !== null) {
        showExplanation();
    }
}

// اختيار إجابة - مقفل بعد الاختيار
function selectAnswer(answerIndex) {
    // إذا كان السؤال مقفولاً بالفعل، لا تفعل شيئاً
    if (answerLocked[currentQuestionIndex]) {
        return;
    }
    
    userAnswers[currentQuestionIndex] = answerIndex;
    answerLocked[currentQuestionIndex] = true;
    // تعطيل جميع خيارات الراديو في السؤال الحالي
    const radioInputs = document.querySelectorAll(`input[name="q${currentQuestionIndex}"]`);
    radioInputs.forEach(input => {
        input.disabled = true;
        input.onclick = function(e) {
            e.preventDefault();
            return false;
        };
    });
    
    // إضافة فئة locked لجميع labels
    const labels = document.querySelectorAll(`input[name="q${currentQuestionIndex}"]`);
    labels.forEach(input => {
        input.closest('label').classList.add('locked');
    });
    
    // إظهار الشرح والتغذية الراجعة
    showExplanation();
    // تحديث قائمة الأسئلة إذا كانت ظاهرة
    if (document.getElementById('questions-overlay').style.display === 'block') {
        showQuestionsList();
    }
    // إضافة تأثير بصرية للإشارة إلى أن الإجابة مقفولة
    const questionNumber = document.querySelector('.question-number');
    if (questionNumber) {
        const lockSpan = document.createElement('span');
        lockSpan.innerHTML = '<i class="fas fa-lock" style="margin-right: 8px;"></i>تم قفل الإجابة';
        lockSpan.style.color = 'var(--accent)';
        lockSpan.style.marginRight = '10px';
        lockSpan.style.fontSize = '0.9em';
        lockSpan.style.animation = 'fadeIn 0.5s ease';
        questionNumber.appendChild(lockSpan);
        
        // إخفاء الرسالة بعد 3 ثوان
        setTimeout(() => {
            if (lockSpan.parentNode) {
                lockSpan.style.opacity = '0';
                lockSpan.style.transition = 'opacity 0.5s ease';
                setTimeout(() => {
                    if (lockSpan.parentNode) {
                        lockSpan.parentNode.removeChild(lockSpan);
                    }
                }, 500);
            }
        }, 3000);
    }
}

// عرض الشرح
function showExplanation() {
    const question = questions[currentQuestionIndex];
    const explanationDiv = document.getElementById("explanation");
    const userAnswer = userAnswers[currentQuestionIndex];
    
    if (userAnswer !== null) {
        explanationDiv.style.display = "block";
        
        let resultHTML = "";
        
        if (userAnswer === question.answer) {
            resultHTML = `<p class="correct"><i class="fas fa-check-circle"></i> إجابة صحيحة</p>`;
        } else {
            resultHTML = `
                <p class="wrong"><i class="fas fa-times-circle"></i> إجابة خاطئة — الإجابة الصحيحة: <span class="correct">${question.options[question.answer]}</span></p>
            `;
        }
        
        // إضافة الشروح الملونة
        resultHTML += `
            <div class="explanation-line explanation-correct"><strong>التفسير الصحيح:</strong> ${question.explanations.correct}</div>
        `;
        
        // إضافة التفسيرات للخيارات الخاطئة
        const wrongKeys = ['wrong1', 'wrong2', 'wrong3'];
        const colors = ['explanation-wrong-1', 'explanation-wrong-2', 'explanation-wrong-3'];
        
        wrongKeys.forEach((key, index) => {
            if (question.explanations[key]) {
                resultHTML += `<div class="explanation-line ${colors[index]}">${question.explanations[key]}</div>`;
            }
        });
        
        explanationDiv.innerHTML = resultHTML;
    }
}

// الانتقال إلى السؤال التالي
function nextQuestion() {
    if (currentQuestionIndex < questions.length - 1) {
        currentQuestionIndex++;
        loadQuiz();
    }
}

// الانتقال إلى السؤال السابق
function previousQuestion() {
    if (currentQuestionIndex > 0) {
        currentQuestionIndex--;
        loadQuiz();
    }
}

// عرض الدرجات الحالية دون إنهاء الاختبار
function showCurrentScore() {
    let totalCorrect = 0;
    userAnswers.forEach((answer, index) => {
        if (answer === questions[index]?.answer) {
            totalCorrect++;
        }
    });
    
    const total = questions.length;
    const percentage = total > 0 ? ((totalCorrect / total) * 100).toFixed(2) : 0;
    
    document.getElementById("current-score").style.display = "block";
    document.getElementById("current-correct").innerHTML = `الإجابات الصحيحة: ${totalCorrect} من ${total}`;
    document.getElementById("current-percentage").innerHTML = `النسبة المئوية الحالية: ${percentage}%`;
}

// حساب الدرجات النهائية
function finishQuiz() {
    clearInterval(timerInterval);
    
    let totalCorrect = 0;
    userAnswers.forEach((answer, index) => {
        if (answer === questions[index]?.answer) {
            totalCorrect++;
        }
    });
    
    const total = questions.length;
    const percentage = total > 0 ? ((totalCorrect / total) * 100).toFixed(2) : 0;
    
    let evaluation = "";
    let evaluationIcon = "";
    if (percentage >= 90) {
        evaluation = "ممتاز";
        evaluationIcon = "🌟";
    } else if (percentage >= 80) {
        evaluation = "جيد جداً";
        evaluationIcon = "🔵";
    } else if (percentage >= 70) {
        evaluation = "جيد";
        evaluationIcon = "🟢";
    } else {
        evaluation = "يحتاج تحسين";
        evaluationIcon = "⚠️";
    }
    
    document.getElementById("result-box").style.display = "block";
    document.getElementById("result").innerHTML = `${evaluationIcon} النتيجة: ${totalCorrect} من ${total}`;
    document.getElementById("percentage").innerHTML = `النسبة المئوية: ${percentage}%`;
    document.getElementById("evaluation").innerHTML = `التقييم: ${evaluation}`;
    
    // إخفاء الاختبار
    document.getElementById("quiz").style.display = "none";
    document.querySelector(".controls").style.display = "none";
    hideQuestionsList();
}

// إبدأ الاختبار 
function addSampleQuestions() {
    // إضافة جميع الأسئلة الـ 68
    questions.push(
        {
            "id": 1,
            "q": "ما يميز الفرد في مرحلة العمليات الحسية عند بياجيه:",
            "options": ["النمو اللغوي", "التفكير المجرد", "النمو الحسي الحركي", "التصنيف والترتيب"],
            "answer": 2,
            "explanations": {
                "correct": "النمو الحسي الحركي هو ما يميز مرحلة العمليات الحسية عند بياجيه، حيث يعتمد الطفل على الحواس والحركة لاكتساب المعرفة وفهم العالم من حوله.",
                "wrong1": "النمو اللغوي يحدث تدريجيًا عبر مراحل الطفولة، لكنه ليس ما يميز مرحلة العمليات الحسية بشكل رئيسي. مثال: الطفل قد يتعلم كلمات ولكنه لا يستطيع التفكير المجرد بعد.",
                "wrong2": "التفكير المجرد يظهر في مرحلة العمليات العقلية الرسمية لاحقاً، وليس في مرحلة العمليات الحسية، حيث يفكر الطفل بشكل ملموس وحسي.",
                "wrong3": "التصنيف والترتيب جزء من مرحلة العمليات العقلية العملية، أي تأتي بعد مرحلة العمليات الحسية، حيث يبدأ الطفل بقدرة على ترتيب الأشياء وتصنيفها."
            }
        },
        {
            "id": 2,
            "q": "القاسم المشترك الأكبر للأعداد ٥٦ و٢١:",
            "options": ["6", "7", "8", "9"],
            "answer": 1,
            "explanations": {
                "correct": "القاسم المشترك الأكبر بين ٥٦ و٢١ هو 7، لأنه العدد الأكبر الذي يقسم كلا الرقمين بدون باقي.",
                "wrong1": "6 لا يقسم 21 بدون باقي، لذا لا يمكن أن يكون القاسم المشترك الأكبر.",
                "wrong2": "8 يقسم 56 لكنه لا يقسم 21، لذا غير صحيح.",
                "wrong3": "9 لا يقسم أيًّا من الرقمين بشكل صحيح، لذا ليس القاسم المشترك الأكبر."
            }
        },
        {
            "id": 3,
            "q": "يستخدم معلم اللغة العربية طريقة المناظرة في إحدى القضايا المجتمعية؛ حيث يقسم الطلاب إلى مؤيدين ومعارضين ويستعين بمحكمين مستقلين، يهدف إلى تنمية:",
            "options": ["اتخاذ القرار", "التفكير الناقد", "التفكير الإبداعي", "حل المشكلات"],
            "answer": 1,
            "explanations": {
                "correct": "المناظرة تهدف لتنمية التفكير الناقد، حيث يقوم الطلاب بتحليل الأدلة، تقييم الحجج، وتحديد موقفهم بناءً على تحليل منطقي.",
                "wrong1": "اتخاذ القرار قد يكون نتيجة للمناظرة، لكنه ليس الهدف الرئيسي، لأن المناظرة تركز على التحليل النقدي والحجج.",
                "wrong2": "التفكير الإبداعي مرتبط بالابتكار وحل المشكلات بطرق جديدة، وليس التركيز على تقييم الأدلة والحجج كما في المناظرة.",
                "wrong3": "حل المشكلات قد يكون نتيجة جانبية، لكنه ليس جوهر النشاط التربوي في المناظرة."
            }
        },
        {
            "id": 4,
            "q": "الفعل الذي يدل على مستوى التركيب هو:",
            "options": ["يعرف", "يقارن", "يوضح", "يقترح"],
            "answer": 1,
            "explanations": {
                "correct": "'يقارن' يدل على مستوى التركيب في تصنيف بلوم، لأنه يتطلب دمج المعلومات والمفاهيم المختلفة لتكوين فهم أعمق.",
                "wrong1": "'يعرف' يشير إلى مستوى المعرفة أو التذكر، أي القدرة على استدعاء معلومات محددة دون دمجها.",
                "wrong2": "'يوضح' ينتمي إلى مستوى الفهم، حيث يفسر المعلومات أو يشرحها للآخرين.",
                "wrong3": "'يقترح' يمكن أن يكون على مستوى الإبداع أو التقويم، لكنه ليس التركيب بالمعنى الأكاديمي المصنف في التعليم."
            }
        },
        {
            "id": 5,
            "q": "غرفة مربعة طولها 8م وارتفاعها 3م، إذا أردنا تغطية جدارين بالقماش فكم نحتاج؟",
            "options": ["36", "42", "48", "56"],
            "answer": 2,
            "explanations": {
                "correct": "مساحة الجدار الواحد = الطول × الارتفاع = 8 × 3 = 24 م²، ولجدارين = 24 × 2 = 48 م²، إذن نحتاج 48 م² من القماش.",
                "wrong1": "36 م² خاطئة، ربما تم حساب الطول مضروباً بارتفاع أقل أو نسيت أحد الجدران.",
                "wrong2": "42 م² خاطئة، رقم غير دقيق من الحساب.",
                "wrong3": "56 م² خاطئة، ربما حسب الجدران الأربعة أو أضاف مساحة إضافية غير مطلوبة."
            }
        },
        {
            "id": 6,
            "q": "فن أدبي يعبر عن فكرة تطرأ على بال الكاتب، ولا تحتاج إلى إعداد مسبق:",
            "options": ["القصة", "المقالة", "الرسالة", "الخاطرة"],
            "answer": 3,
            "explanations": {
                "correct": "الخاطرة هي تعبير أدبي قصير يظهر الفكرة أو الانطباع فورًا دون إعداد مسبق، وغالبًا ما يعكس مشاعر الكاتب.",
                "wrong1": "القصة تحتاج إلى إعداد، حبكة، وشخصيات، فهي ليست فورية مثل الخاطرة.",
                "wrong2": "المقالة تتطلب جمع معلومات وتنظيم الأفكار، لذا لا تصنف كخاطرة.",
                "wrong3": "الرسالة وسيلة تواصل محددة، تتطلب صياغة وهدف واضح، وليست مجرد انطباع لحظي."
            }
        },
        {
            "id": 7,
            "q": "يستخدم معامل كرونباخ لمعرفة:",
            "options": ["صدق الأداة", "ثبات الأداة", "العلاقة النسبية", "العلاقة الاسمية"],
            "answer": 1,
            "explanations": {
                "correct": "معامل كرونباخ يستخدم لقياس ثبات الأداة أي درجة الاتساق الداخلي للاختبار أو الاستبانة، ويشير إلى مدى موثوقية النتائج.",
                "wrong1": "صدق الأداة يقيس مدى قدرة الاختبار على قياس ما صُمم لقياسه، وليس دوره في معامل كرونباخ.",
                "wrong2": "العلاقة النسبية لا علاقة لها بمعامل كرونباخ، هي تتعلق بالارتباط بين متغيرين.",
                "wrong3": "العلاقة الاسمية تخص تصنيف البيانات الفئوية ولا تدخل في ثبات الأداة."
            }
        },
        {
            "id": 8,
            "q": "معلم استخدم صورة لنبات لعرض أجزائه؛ حسب مخروط ديل نوع الخبرات هو:",
            "options": ["مباشرة", "غير مباشرة", "مجردة", "شبه رمزية"],
            "answer": 3,
            "explanations": {
                "correct": "التجربة شبه الرمزية هي استخدام صور أو رموز تمثل الواقع بشكل غير مباشر، كما في صورة النبات لتوضيح الأجزاء.",
                "wrong1": "المباشرة تعني خبرة حسية مباشرة مع الشيء نفسه، مثل لمس النبات.",
                "wrong2": "غير مباشرة تشير إلى خبرة مستخلصة من تجربة الآخرين، مثل مشاهدة فيديو لشخص يشرح النبات.",
                "wrong3": "مجردة تشير إلى المفاهيم النظرية دون أي تمثيل بصري، مثل شرح أجزاء النبات بالكلمات فقط."
            }
        },
        {
            "id": 9,
            "q": "الديسلكسيا مصطلح في مجال صعوبات التعلم يشير تحديدًا إلى:",
            "options": ["عسر القراءة", "اضطرابات انفعالية", "الحسبة الكلامية النمائية", "الاختلال الوظيفي الدماغي"],
            "answer": 0,
            "explanations": {
                "correct": "الديسلكسيا تعني عسر القراءة، وهي صعوبة تعلم القراءة رغم ذكاء طبيعي وبيئة تعليمية مناسبة.",
                "wrong1": "الاضطرابات الانفعالية تتعلق بسلوك الطالب ومشاعره، وليست ديسلكسيا.",
                "wrong2": "الحسبة الكلامية النمائية تتعلق بالرياضيات والكلمات، وليست مرتبطة بالقراءة.",
                "wrong3": "الاختلال الوظيفي الدماغي عام وقد يشمل جوانب أخرى، بينما الديسلكسيا محددة بالقراءة."
            }
        },
        {
            "id": 10,
            "q": "شاهدت في البئر:",
            "options": ["مائن", "ماءاً", "ماا", "ماء"],
            "answer": 3,
            "explanations": {
                "correct": "الكلمة الصحيحة إملائيًا هي 'ماء'.",
                "wrong1": "'مائن' خاطئة لأنها لفظ مختلف ولا تتوافق مع معنى الجملة.",
                "wrong2": "'ماءاً' خاطئة، إضافة الألف والنون غير صحيحة نحوياً.",
                "wrong3": "'ماا' خاطئة، لأنه خطأ إملائي واضح ويكرر حرف الألف."
            }
        },
        {
            "id": 11,
            "q": "طالب زعل زميله في الفصل، وخرب المقعد، تم تحويله للمرشد وطلب منه الاعتذار ووضع كرسي جديد؛ ما الأسلوب الذي استخدمه المرشد؟",
            "options": ["إقصاء", "تصحيح زائد", "تكلفة الاستجابة", "التعزيز السلبي"],
            "answer": 2,
            "explanations": {
                "correct": "تكلفة الاستجابة هي أسلوب تربوي يعاقب الطالب على سلوك خاطئ بإلزامه بسلوك تصحيحي مرتبط بالخطأ، مثل إصلاح المقعد.",
                "wrong1": "الإقصاء يعني منع الطالب من المشاركة أو عزله عن النشاط، وليس طلب إصلاح الخطأ.",
                "wrong2": "تصحيح زائد يكون بإضافة مهام إضافية غير مرتبطة مباشرة بالسلوك الخاطئ.",
                "wrong3": "التعزيز السلبي يستخدم لسحب عامل مريح لتقوية السلوك، وليس لإصلاح الخطأ بشكل مباشر."
            }
        },
        {
            "id": 12,
            "q": "معلم رياضيات يرغب التأكد من إتقان طلابه الضرب قبل الانتقال إلى القسمة؛ أي اختبار يستخدم؟",
            "options": ["الرأسي", "الأفقي", "السالب", "الصفري"],
            "answer": 0,
            "explanations": {
                "correct": "الاختبار الرأسي يقيس مستويات متتابعة من التعلم، بحيث يجب إتقان مرحلة قبل الانتقال للأخرى.",
                "wrong1": "الاختبار الأفقي يقارن أداء الطلاب في نفس المستوى وليس بالتتابع.",
                "wrong2": "الاختبار السالب غير مستخدم في هذا السياق.",
                "wrong3": "الاختبار الصفري يستخدم عادة لتحديد المعرفة السابقة، وليس للتحقق من الإتقان قبل الانتقال للمرحلة التالية."
            }
        },
        {
            "id": 13,
            "q": "معلمة اعتقدت أن الاختبار الدولي يحتاج وقتًا أطول، فأعطت الطالبات 10 دقائق إضافية دون أن تخبر أحدًا؛ إن ما قامت به المعلمة:",
            "options": ["انتهاك ضوابط الاختبار", "لا يؤثر على نتائج الاختبار", "تصرف صحيح نابع من حرصها على الطالبات"],
            "answer": 0,
            "explanations": {
                "correct": "إعطاء وقت إضافي دون تصريح رسمي يعد انتهاكًا لضوابط الاختبار، وقد يؤثر على موثوقية النتائج ومصداقية القياس.",
                "wrong1": "لا يؤثر على النتائج: هذا غير صحيح، لأن الوقت الإضافي قد يعطي بعض الطالبات ميزة غير عادلة.",
                "wrong2": "تصرف صحيح: حتى لو كان نابعًا من حرصها، فهذا لا يبرر مخالفة التعليمات الرسمية."
            }
        },
        {
            "id": 14,
            "q": "يتعاون المعلمون في المدرسة بشكل تبادلي من أجل تطوير أدائهم والتنمية المستدامة من خلال:",
            "options": ["مراجعة المادة المدرسية", "مجتمعات التعلم المهنية", "التعاون مع المدير", "التخطيط المستمر والفعال"],
            "answer": 1,
            "explanations": {
                "correct": "مجتمعات التعلم المهنية هي مجموعات من المعلمين يتبادلون الخبرات ويدعمون بعضهم البعض بهدف تحسين الأداء والتعلم المستدام.",
                "wrong1": "مراجعة المادة المدرسية نشاط فردي أكثر منه تبادلي.",
                "wrong2": "التعاون مع المدير مهم لكنه لا يشمل تبادل الخبرات بين المعلمين بشكل مباشر.",
                "wrong3": "التخطيط المستمر والفعال جزء من العملية التدريسية لكنه لا يمثل مجتمع تعلم مهني تبادلي."
            }
        },
        {
            "id": 15,
            "q": "شعور الطالب بالقلق عند أداء اختبار قياس من منظور سلوكي يمثل هذا الشعور استجابة:",
            "options": ["فطرية", "طبيعية", "شرطية", "لا شيء مما سبق"],
            "answer": 2,
            "explanations": {
                "correct": "من منظور السلوك الشرطي، القلق يعد استجابة مكتسبة نتيجة خبرة معينة مرتبطة بالاختبار (شرطية)، وليس فطرية.",
                "wrong1": "فطرية: القلق ليس مكتسبًا تلقائيًا، بل يكون مرتبطًا بالموقف.",
                "wrong2": "طبيعية: القلق في هذا السياق ليس مجرد شعور طبيعي بل استجابة متعلمة.",
                "wrong3": "لا شيء مما سبق: هذا غير صحيح، لأنه ينتمي للتفسير الشرطي للسلوك."
            }
        },
        {
            "id": 16,
            "q": "آراء طلابك والتغذية الراجعة من زملائك المعلمين كلاهما وسائل لمعرفة وتحديد:",
            "options": ["الأهداف التربوية", "العلاقات الإيجابية", "الصلاحيات التربوية", "الاحتياجات التدريبية"],
            "answer": 3,
            "explanations": {
                "correct": "الاحتياجات التدريبية يمكن تحديدها عبر آراء الطلاب وزملاء المعلمين لمعرفة مجالات القوة والضعف وتطوير الأداء.",
                "wrong1": "الأهداف التربوية تحدد من الإدارة أو المقررات ولا تعتمد فقط على التغذية الراجعة.",
                "wrong2": "العلاقات الإيجابية مهمة، لكنها ليست الهدف من جمع الآراء.",
                "wrong3": "الصلاحيات التربوية تشير إلى سلطات المعلم، وليست مرتبطة مباشرة بتقييم الاحتياجات."
            }
        },
        {
            "id": 17,
            "q": "الفعل «يقارن» ينضم إلى:",
            "options": ["التحليل", "التركيب", "التقويم", "الفهم"],
            "answer": 1,
            "explanations": {
                "correct": "'يقارن' من مستوى التركيب لأنه يتطلب جمع المعلومات والمفاهيم المختلفة ومقارنتها لتكوين فهم أعمق.",
                "wrong1": "التحليل يشمل تفكيك العناصر إلى أجزاء، لكنه لا يدمجها كما في التركيب.",
                "wrong2": "التقويم يشير إلى الحكم على قيمة أو جودة شيء ما، وليس مقارنة المعلومات لبناء تركيب.",
                "wrong3": "الفهم يشمل تفسير المعلومات فقط، وليس دمجها أو مقارنتها."
            }
        },
        {
            "id": 18,
            "q": "إذا كان معامل الارتباط لدرجات الطلاب في اختبارين لمادتين مختلفتين هو 0.8 فإن هذا يعني أن:",
            "options": ["أن 80% من الطلاب نجحوا في الاختبارين", "العلاقة قوية بين المادتين", "الاختبارات تمتاز بالصدق والثبات", "أن الاختبارين يتميزان بالسهولة الشديدة"],
            "answer": 1,
            "explanations": {
                "correct": "معامل الارتباط 0.8 يشير إلى علاقة قوية بين المادتين، أي أن أداء الطلاب في اختبار واحد مرتبط بأدائهم في الاختبار الآخر.",
                "wrong1": "80% من الطلاب نجحوا: هذا تفسير خاطئ لمعامل الارتباط، فهو لا يقيس النسبة المئوية للنجاح.",
                "wrong2": "الاختبارات تمتاز بالصدق والثبات: الصدق والثبات مفهومان مستقلان عن معامل الارتباط.",
                "wrong3": "السهولة الشديدة: معامل الارتباط لا يعكس مستوى الصعوبة."
            }
        },
        {
            "id": 19,
            "q": "استخدم المعلم استراتيجية ما وراء المعرفة، بدأ بعرض الموضوع، ثم جعل الطلاب يسألون أنفسهم، ثم ناقشهم بالمعلومات التي لديهم، ثم حللوا وقيّموا؛ الاستراتيجية هي:",
            "options": ["العصف الذهني", "التساؤل الذاتي", "النمذجة", "فكر/زاوج/شارك"],
            "answer": 1,
            "explanations": {
                "correct": "التساؤل الذاتي يهدف إلى جعل الطالب يسأل نفسه ويفكر في المعلومات المتاحة، ثم يصل إلى استنتاجات، وهو ما يصفه المثال.",
                "wrong1": "العصف الذهني يركز على توليد الأفكار الإبداعية الجماعية، وليس على التفكير الفردي الذاتي.",
                "wrong2": "النمذجة هي عرض سلوك أو مهارة لتقليده من قبل الطلاب، وليست استراتيجية للتساؤل الذاتي.",
                "wrong3": "فكر/زاوج/شارك يركز على النقاش بين الطلاب وليس على التفكير الداخلي الفردي."
            }
        },
        {
            "id": 20,
            "q": "معلم يطبق نموذج المنظم المتقدم، وكلف الطلاب بتحديد النقاط والجوانب التي فيها اختلاف أو تشابه بين المفاهيم؛ أي عمليات التعلم ذي المعنى يستهدف؟",
            "options": ["الدعم والتسقيل", "التوفيق التكاملي", "التمايز التقدمي", "التنظيم المتسلسل"],
            "answer": 1,
            "explanations": {
                "correct": "التوفيق التكاملي يركز على دمج المفاهيم المختلفة ومعرفة أوجه التشابه والاختلاف بينها، وهو ما طبقه المعلم.",
                "wrong1": "الدعم والتسقيل يركز على تعزيز التعلم السابق، وليس المقارنة بين المفاهيم.",
                "wrong2": "التمايز التقدمي يهتم بتقديم معلومات معقدة تدريجيًا، وليس التركيز على الاختلاف والتشابه.",
                "wrong3": "التنظيم المتسلسل يركز على ترتيب المعلومات بشكل متتابع، وليس على المقارنة بين المفاهيم."
            }
        },
        {
            "id": 21,
            "q": "معلم جمع لطلابه أحاديث عن الجار، وطلب منهم استخراج قاعدة مشتركة منها؛ هذا يعد:",
            "options": ["قياس", "استقراء", "اكتشاف", "تعلم موجّه"],
            "answer": 1,
            "explanations": {
                "correct": "الاستقراء هو استنتاج قاعدة عامة من أمثلة محددة، كما في المثال حيث يستخلص الطلاب قاعدة من أحاديث متعددة.",
                "wrong1": "القياس يشير إلى تطبيق قاعدة عامة على حالة جديدة، وليس استخراج القاعدة.",
                "wrong2": "الاكتشاف يشمل التعرف على شيء جديد بشكل فردي دون توجيه مباشر، بينما هنا النشاط موجه.",
                "wrong3": "التعلم الموجّه يكون بتقديم قاعدة مباشرة للطلاب دون استخلاصها بأنفسهم."
            }
        },
        {
            "id": 22,
            "q": "معلم يقدم فيديو ومعلومات للدرس ليشاهدها الطالب في منزله، ثم يستثمر وقت الحصة في الاستنتاجات والتعزيز والتفاعل؛ هذه طريقة:",
            "options": ["الفيديو التفاعلي", "الصف المقلوب", "التعليم المدمج", "التعليم المبرمج"],
            "answer": 1,
            "explanations": {
                "correct": "الصف المقلوب يعني مشاهدة الطلاب للدرس في المنزل واستغلال وقت الحصة للنقاش والتطبيق والتفاعل.",
                "wrong1": "الفيديو التفاعلي يركز على التفاعل أثناء مشاهدة الفيديو، وليس هيكلة الحصة بالكامل.",
                "wrong2": "التعليم المدمج يجمع بين التعلم وجهاً لوجه وأونلاين، لكنه لا يشترط الصف المقلوب.",
                "wrong3": "التعليم المبرمج يعتمد على تسلسل المحتوى وتقديمه خطوة بخطوة، وليس على تحويل المشاهدة للمنزل."
            }
        },
        {
            "id": 23,
            "q": "من الأسباب المؤدية إلى عدم فهم النصوص:",
            "options": ["وجود المترادفات اللغوية", "وجود جمل متعددة حول فكرة واحدة", "الاعتماد على الجمل الطويلة", "الاقتصار على الجمل الخبرية"],
            "answer": 2,
            "explanations": {
                "correct": "الجمل الطويلة والمعقدة تجعل فهم النصوص صعبًا، لأنها تزيد الحمل المعرفي على الطالب.",
                "wrong1": "المترادفات اللغوية قد تسبب بعض الالتباس لكن ليست السبب الرئيسي.",
                "wrong2": "الجمل المتعددة حول فكرة واحدة قد تساعد على التوضيح أكثر من التعقيد.",
                "wrong3": "الاقتصار على الجمل الخبرية يقلل من صعوبة النص، لا يزيدها."
            }
        },
        {
            "id": 24,
            "q": "ورد تعميم عن وجوب المحافظة على مواقع الآثار والتراث العمراني وعدم إصدار رخص البناء أو الترميم إلا بعد موافقة وزارة السياحة؛ أي نشاط غير صفي لا يصلح لتعزيز هذه القضية؟",
            "options": ["حث أصحاب المباني التراثية على تجديد مظهرها", "تقديم مبادرات لتحويل المباني التراثية إلى مبان حديثة", "إعداد فيلم وثائقي عن المباني التراثية في الحي", "توزيع مطويات للتوعية بأهمية المباني التراثية"],
            "answer": 1,
            "explanations": {
                "correct": "تقديم مبان حديثة بدل المباني التراثية يخالف الهدف، فهو يعزز إزالة التراث بدلاً من الحفاظ عليه.",
                "wrong1": "حث أصحاب المباني يعزز المحافظة على التراث.",
                "wrong2": "إعداد فيلم وثائقي يرفع الوعي ويعزز قيمة التراث.",
                "wrong3": "توزيع مطويات وسيلة تعليمية للتوعية العامة."
            }
        },
        {
            "id": 25,
            "q": "كلف المعلم طلابه بنشاط تعليمي تتطلب مراحله توليد تخمينات ذكية؛ أي استراتيجية طبق؟",
            "options": ["حل المشكلات", "التعلم الإتقاني", "التعلم بالاكتشاف", "الذكاءات المتعددة"],
            "answer": 2,
            "explanations": {
                "correct": "التعلم بالاكتشاف يركز على نشاط الطلاب لتوليد استنتاجات وتخمينات بناءً على خبراتهم وملاحظاتهم.",
                "wrong1": "حل المشكلات قد يتطلب خطوات محددة مسبقة، لكنه لا يركز على الاكتشاف الذاتي.",
                "wrong2": "التعلم الإتقاني يركز على إتقان مهارة محددة بشكل تدريجي.",
                "wrong3": "الذكاءات المتعددة نظرية حول أساليب تعلم الطلاب، وليست استراتيجية عملية."
            }
        },
        {
            "id": 26,
            "q": "يُسرف بعض الشباب في تناول الأطعمة سريعة التحضير، رغم أن البحث العلمي أثبت أن الاستهلاك المفرط لهذه الأطعمة ضار بصحته، ومن أكبر مشكلاته. «أليس داء السكري أحد نتائج ذلك؟» الضمير «ه» في جملة «ومن أكبر مشكلاته» يعود على:",
            "options": ["الطعام سريع التحضير", "الاستهلاك المفرط", "الإنسان المعاصر", "بعض الشباب"],
            "answer": 1,
            "explanations": {
                "correct": "الضمير 'ه' يعود على 'الاستهلاك المفرط'، لأنه الموضوع المباشر لمشكلة الصحة المذكورة.",
                "wrong1": "الطعام سريع التحضير عام، لكن المشكلة مرتبطة بالإفراط في الاستهلاك.",
                "wrong2": "الإنسان المعاصر عام جدًا، لا يشير مباشرة إلى المشكلة.",
                "wrong3": "بعض الشباب يشير إلى الفاعل، لكن الضمير يعود على السبب (الاستهلاك المفرط)."
            }
        },
        {
            "id": 27,
            "q": "تعتمد الشراكة بين المدرسة والمجتمع على العديد من الأطراف مثل إدارة المدرسة، أولياء أمور الطلاب، بعض القطاعات الحكومية، والقطاع الخاص، والجامعات، ويعتمد نجاح الشراكة على الاحترام المتبادل وتقدير جهود المعلمين وتعزيز المسؤولية المتبادلة؛ ما سبق يعني:",
            "options": ["مقومات الشراكة بين المدرسة والأسرة والمجتمع", "خصائص الشراكة المجتمعية بين الأسرة والمدرسة", "المسؤولية المجتمعية وعلاقتها بالشراكة المجتمعية", "متطلبات تفصيل الشراكة بين المدرسة والأسرة والمجتمع"],
            "answer": 0,
            "explanations": {
                "correct": "مقومات الشراكة تشير إلى العناصر الأساسية لنجاح التعاون بين المدرسة والمجتمع، كما هو موضح.",
                "wrong1": "خصائص الشراكة تركز على طبيعة الشراكة وليست مقوماتها الأساسية.",
                "wrong2": "المسؤولية المجتمعية جزء من المقومات، لكنها لا تشمل كل العناصر.",
                "wrong3": "متطلبات تفصيل الشراكة يعني خطوات عملية، بينما السؤال يركز على المقومات الأساسية."
            }
        },
        {
            "id": 28,
            "q": "يمكن التنبؤ بأن درجات الطالب الحاصل على درجة اختبار ذكاء 110 بأنها:",
            "options": ["تبقى كما هي 110", "تتغير بالتقدم بالعمر فقط", "ترتفع بالخبرات المنظمة", "تنخفض بالتقدم بالعمر"],
            "answer": 2,
            "explanations": {
                "correct": "الخبرات المنظمة والتعلم يمكن أن تؤثر على أداء الطالب وزيادة مهاراته، وبالتالي تحسين درجاته في اختبارات الذكاء.",
                "wrong1": "تبقى كما هي: الذكاء ليس ثابتًا تمامًا، بل يتأثر بالخبرة.",
                "wrong2": "تتغير بالعمر فقط: العمر وحده لا يكفي لتغيير الدرجة.",
                "wrong3": "تنخفض بالعمر: هذا غير صحيح للطفل واليافعين؛ الانخفاض يحدث عادة في مراحل متقدمة من العمر."
            }
        },
        {
            "id": 29,
            "q": "يُنسب الإطفاء إلى نظرية الاشتراط:",
            "options": ["الاشتراط البسيط", "الاشتراط الإجرائي", "الإنساني", "التعزيز"],
            "answer": 1,
            "explanations": {
                "correct": "الإطفاء (Extinction) هو مصطلح في الاشتراط الإجرائي يشير إلى تلاشي استجابة معينة عند إزالة التعزيز.",
                "wrong1": "الاشتراط البسيط (الكلاسيكي) يستخدم مصطلحات أخرى مثل الشرطية والاستجابة غير المشروطة.",
                "wrong2": "النظرية الإنسانية تركز على الاحتياجات النفسية، وليست مرتبطة بالإطفاء.",
                "wrong3": "التعزيز هو عملية زيادة السلوك، وليس إلغاؤه."
            }
        },
        {
            "id": 30,
            "q": "قدّم معلم درسه باتباع هذه الخطوات: (مرحلة الاكتشاف – مرحلة تقديم المفهوم – مرحلة تطبيق المفهوم)، الاستراتيجية التي نفذها المعلم:",
            "options": ["دورة التعلم", "الاستقصاء", "الاستنتاج", "لا شيء مما ذكر"],
            "answer": 1,
            "explanations": {
                "correct": "الاستقصاء يشمل الاكتشاف، ثم تقديم المفاهيم، ثم التطبيق؛ وهو ما وصفه المعلم في المثال.",
                "wrong1": "دورة التعلم يشير إلى نموذج عام للتعلم وليس الطريقة التفصيلية هذه.",
                "wrong2": "الاستنتاج يركز على الوصول للنتيجة النهائية، وليس المراحل الثلاث المتكاملة.",
                "wrong3": "لا شيء مما ذكر: غير صحيح، لأن الخطوات تتوافق مع استراتيجية الاستقصاء."
            }
        },
        {
            "id": 31,
            "q": "ما هو المدى فيما يلي: 8، 7، 6، 5، 4، 8، 9، 20؟",
            "options": ["8", "1", "9", "16"],
            "answer": 3,
            "explanations": {
                "correct": "المدى هو الفرق بين أكبر وأصغر قيمة: 20 - 4 = 16.",
                "wrong1": "8 هو الفرق بين أكبر قيمة في البيانات المكررة، لكن لا يمثل المدى.",
                "wrong2": "1 هو الفرق بين الأعداد المتتالية في بعض الأحيان وليس المدى العام.",
                "wrong3": "9 خطأ حسابي؛ المدى يحسب باستخدام أكبر وأصغر قيمة فقط."
            }
        },
        {
            "id": 32,
            "q": "الكلمة الصحيحة إملائيًا فيما يأتي:",
            "options": ["مكافآة", "مكافاءة", "مكافأة", "مكافاة"],
            "answer": 2,
            "explanations": {
                "correct": "'مكافأة' هي الكتابة الصحيحة وفق قواعد الإملاء العربية.",
                "wrong1": "مكافآة: الخطأ في وضع الألف المقصورة.",
                "wrong2": "مكافاءة: الخطأ في استخدام الألف قبل الهاء.",
                "wrong3": "مكافاة: الحذف الخاطئ للياء."
            }
        },
        {
            "id": 33,
            "q": "فصل فيه 35 طالبًا، و28 طالبًا سلموا الواجب، كم نسبة الذين لم يسلموا؟",
            "options": ["7%", "10%", "20%", "30%"],
            "answer": 2,
            "explanations": {
                "correct": "عدد الطلاب الذين لم يسلموا = 35 - 28 = 7. النسبة = (7/35)*100 = 20%.",
                "wrong1": "7%: خطأ في تحويل العدد إلى نسبة.",
                "wrong2": "10%: حساب خاطئ.",
                "wrong3": "30%: تقدير مبالغ فيه."
            }
        },
        {
            "id": 34,
            "q": "فاطمة تجمع 9 ريالات كل 15 يومًا، فكم تحتاج يومًا لتصل إلى 45 ريالًا؟",
            "options": ["15", "30", "75", "90"],
            "answer": 2,
            "explanations": {
                "correct": "تحصل على 9 ريالات كل 15 يومًا، للوصول إلى 45 ريالًا: 45 ÷ 9 = 5 مرات. 5 × 15 يوم = 75 يوم.",
                "wrong1": "15 يوم: لا يكفي أبداً.",
                "wrong2": "30 يوم: غير كافٍ.",
                "wrong3": "90 يوم: أكثر من اللازم."
            }
        },
        {
            "id": 35,
            "q": "يتم منح الطلاب مهمة صعبة ثم يطلب المعلم منهم الإجابة عنها شفهيًا أو كتابيًا، يسمى هذا النوع من التقييم بـ:",
            "options": ["البورتفيوليو", "تقييم الأداء", "التقييم الجمعي", "التقييم مفتوح النهاية"],
            "answer": 1,
            "explanations": {
                "correct": "تقييم الأداء يركز على قدرات الطالب على تطبيق المعرفة والمهارات في مهام عملية أو أداء.",
                "wrong1": "البورتفيوليو هو ملف إنجازات الطالب خلال فترة زمنية.",
                "wrong2": "التقييم الجمعي يقيس أداء مجموعة وليس فرديًا.",
                "wrong3": "التقييم مفتوح النهاية يشمل أسئلة غير محددة، لكنه لا يشير بالضرورة إلى الأداء العملي."
            }
        },
        {
            "id": 36,
            "q": "تظهر عيوب القراءة من خلال القراءة:",
            "options": ["السريعة", "المتأنية", "الجهرية", "الصامتة"],
            "answer": 2,
            "explanations": {
                "correct": "القراءة الجهرية تسمح للمعلم برصد العيوب مثل الأخطاء في النطق أو التلعثم.",
                "wrong1": "السريعة قد تخفي العيوب لأنها لا تركز على النطق.",
                "wrong2": "المتأنية تساعد على الفهم، لكن لا تظهر الأخطاء الشفهية بسهولة.",
                "wrong3": "الصامتة لا يمكن للمعلم تقييم النطق أو الأخطاء بشكل مباشر."
            }
        },
        {
            "id": 37,
            "q": "يا سعاد، هل (…….) الدرس؟ الكلمة المناسبة للفراغ:",
            "options": ["أقرءتي", "قرأتي", "قرأتِ", "قرءت"],
            "answer": 2,
            "explanations": {
                "correct": "قرأتِ هي الصياغة الصحيحة للسؤال الموجه للفتاة مع علامة التاء المربوطة.",
                "wrong1": "أقرءتي: صياغة غير صحيحة لغويًا.",
                "wrong2": "قرأتي: ناقصة التشكيل الصحيح.",
                "wrong3": "قرءت: خطأ إملائي."
            }
        },
        {
            "id": 38,
            "q": "من صعوبات التعلم النمائية لدى الطلاب صعوبات:",
            "options": ["القراءة", "الإدراك", "الحساب", "الإحساس"],
            "answer": 0,
            "explanations": {
                "correct": "القراءة من أكثر صعوبات التعلم النمائية شيوعًا بين الطلاب.",
                "wrong1": "الإدراك: مشكلة عامة وليست محددة بالتعلم النمائي.",
                "wrong2": "الحساب: صحيح أحيانًا لكنه أقل شيوعًا من القراءة.",
                "wrong3": "الإحساس: ليس صعوبة تعلم نمائية."
            }
        },
        {
            "id": 39,
            "q": "ناقش مجموعة من المعلمين دورهم في عملية التعليم، فوردت الآراء الآتية؛ أيها يتوافق مع النظرية التربوية المعاصرة؟",
            "options": ["تيسير الفهم", "نقل المعرفة للطلاب", "تحديد موضوعات المقرر", "العمل كمصدر للمعلومات"],
            "answer": 0,
            "explanations": {
                "correct": "النظرية التربوية المعاصرة تركز على توجيه الطلاب لتكوين فهمهم بأنفسهم وليس مجرد نقل المعرفة.",
                "wrong1": "نقل المعرفة يركز على الطريقة التقليدية.",
                "wrong2": "تحديد موضوعات المقرر ليس هدفًا تربويًا مباشرًا للتعليم المعاصر.",
                "wrong3": "العمل كمصدر للمعلومات تقليدي ويقلل دور الطلاب في التعلم الفعال."
            }
        },
        {
            "id": 40,
            "q": "جميع ما يأتي من مداخل التدريس المعرفية عدا:",
            "options": ["الاستقراء", "المحاكاة", "الاستنباط", "حل المشكلات"],
            "answer": 1,
            "explanations": {
                "correct": "المحاكاة ليست مدخلاً معرفيًا بحتًا بل أداة تعليمية لتقليد السلوك.",
                "wrong1": "الاستقراء مدخل معرفي يعتمد على استخلاص القواعد من الأمثلة.",
                "wrong2": "الاستنباط مدخل معرفي يعتمد على استنتاج النتائج من القواعد العامة.",
                "wrong3": "حل المشكلات مدخل معرفي يركز على التفكير الاستراتيجي."
            }
        },
        {
            "id": 41,
            "q": "الحوسبة المعتمدة على الإنترنت والتي توفر الموارد والبيانات للعمليات الحاسوبية المشتركة تحت الطلب تسمى:",
            "options": ["المتنقلة", "المباشرة", "المشتركة", "السحابية"],
            "answer": 3,
            "explanations": {
                "correct": "الحوسبة السحابية توفر البيانات والموارد للعمليات الحاسوبية عبر الإنترنت عند الطلب.",
                "wrong1": "المتنقلة تشير إلى الأجهزة المحمولة وليست طريقة الحوسبة.",
                "wrong2": "المباشرة تعني الاتصال المباشر وليس تقديم الخدمات السحابية.",
                "wrong3": "المشتركة لا تعني الخدمات السحابية بل مشاركة محددة للموارد."
            }
        },
        {
            "id": 42,
            "q": "صفوة الأفكار التي تُقدَّم بالتقرير تكون في:",
            "options": ["المقدمة", "التحليل", "التمهيد", "الختام"],
            "answer": 3,
            "explanations": {
                "correct": "الختام يحتوي على صوغ الأفكار النهائية والنتائج المستخلصة من التقرير.",
                "wrong1": "المقدمة تعرض الغرض ولا تحتوي على الخلاصة.",
                "wrong2": "التحليل يناقش التفاصيل والبيانات، وليس صوغ الأفكار النهائية.",
                "wrong3": "التمهيد يقدم خلفية أو سياق وليس الخلاصة."
            }
        },
        {
            "id": 43,
            "q": "معلم يشارك في الدورات والدروس النموذجية والمؤتمرات؛ كيف يتم تقويم المعلم؟ عن طريق:",
            "options": ["سجل قصصي", "أدوات الرصد", "سير التعلم", "ملف الإنجاز"],
            "answer": 3,
            "explanations": {
                "correct": "ملف الإنجاز يحتوي على جميع الأنشطة والإنجازات المهنية للمعلم ويستخدم لتقويم الأداء.",
                "wrong1": "السجل القصصي يركز على أحداث محددة وليست شاملة.",
                "wrong2": "أدوات الرصد وسيلة لمتابعة الأداء وليست التقرير الكامل.",
                "wrong3": "سير التعلم يشير إلى تقدم الطالب، لا المعلم."
            }
        },
        {
            "id": 44,
            "q": "….. سيستمر الخلاف بيننا؟",
            "options": ["إلاما", "إلام", "إلامي", "إلى ما"],
            "answer": 3,
            "explanations": {
                "correct": "'إلى ما سيستمر الخلاف' صياغة صحيحة لغويًا.",
                "wrong1": "إلاما: غير صحيحة إملائيًا.",
                "wrong2": "إلام: ناقصة ولا تصلح سياقيًا.",
                "wrong3": "إلامي: خطأ إملائي."
            }
        },
        {
            "id": 45,
            "q": "ارحم الحيوان …. ولا تحمِّله ما لا يطيقه ….. لأنه يحس ويتألم كما تحس وتتألم. علامات الترقيم المناسبة هي:",
            "options": ["()()", ")()(", ")()(", "(-)(-)"],
            "answer": 1,
            "explanations": {
                "correct": "علامات الترقيم المناسبة: )()( لتوضيح الفواصل الصحيحة بين العبارات.",
                "wrong1": "()(): ترتيب غير صحيح للفواصل.",
                "wrong2": ")()(: غير مناسب لغويًا.",
                "wrong3": "(-)(-) تستخدم للتوضيح أو الاقتباس وليست مناسبة هنا."
            }
        },
        {
            "id": 46,
            "q": "أي الكلمات الآتية ليس فيها حرف محذوف؟",
            "options": ["تلك", "هؤلاء", "هذا", "ذلك"],
            "answer": 2,
            "explanations": {
                "correct": "'هذا' مكتوبة كاملة دون حذف أي حرف.",
                "wrong1": "تلك: مكتوبة كاملة أيضًا، لكن السياق غالبًا يقارنها بـ 'هؤلاء'.",
                "wrong2": "هؤلاء: بها حذف حرف الألف من 'هؤلا' حسب الأصل اللغوي.",
                "wrong3": "ذلك: حرف اللام لم يُحذف، لكنها هنا مقارنة لغوية."
            }
        },
        {
            "id": 47,
            "q": "المسافة بين غرفة المديرة والمعلمات 616 م، كم تأخذ المعلمة للوصول إذا كانت تسير بسرعة 4 م في الثانية؟",
            "options": ["55 ثانية", "دقيقة وأربعون ثانية", "دقيقتان و34 ثانية", "ثلاث دقائق"],
            "answer": 2,
            "explanations": {
                "correct": "الزمن = المسافة ÷ السرعة = 616 ÷ 4 = 154 ثانية = 2 دقيقة و34 ثانية.",
                "wrong1": "55 ثانية: خطأ في حساب السرعة.",
                "wrong2": "دقيقة وأربعون ثانية: تقدير خاطئ.",
                "wrong3": "ثلاث دقائق: تقريب غير دقيق."
            }
        },
        {
            "id": 48,
            "q": "أي من الفئات الآتية لديهم حساسية عالية في الاقتراب من الآخرين؟",
            "options": ["الإعاقة العقلية الشديدة", "اضطرابات التواصل", "التوحد", "متلازمة داون"],
            "answer": 2,
            "explanations": {
                "correct": "الأطفال المصابون بالتوحد لديهم حساسية عالية تجاه الاقتراب الجسدي واللمس.",
                "wrong1": "الإعاقة العقلية الشديدة: قد يكون التأثير مختلفاً حسب الفرد.",
                "wrong2": "اضطرابات التواصل: تتعلق بالصوت والكلام وليس بالاقتراب الجسدي بالضرورة.",
                "wrong3": "متلازمة داون: عادةً ليست لديهم حساسية عالية تجاه الاقتراب."
            }
        },
        {
            "id": 49,
            "q": "يشير «مارسيا» في حديثه عن حالات الهوية في مرحلة المراهقة إلى حالات أربع؛ إذا كان لديك طالب يريد أن يصبح طبيبًا لأن والديه يريدان ذلك، فما حالة الهوية التي تنطبق على هذا الموقف؟",
            "options": ["المكبلة", "المشككة", "المؤجلة", "المنجزة"],
            "answer": 0,
            "explanations": {
                "correct": "الهوية المكبلة (Foreclosure) هي قبول قرارات الآخرين دون بحث أو استكشاف شخصي.",
                "wrong1": "المشككة: الطالب يشكك ويبحث لكنه لم يتخذ قرارًا بعد.",
                "wrong2": "المؤجلة: تأجيل اتخاذ القرار بعد استكشاف.",
                "wrong3": "المنجزة: اتخاذ قرار مستند إلى استكشاف وتجربة شخصية."
            }
        },
        {
            "id": 50,
            "q": "قسم المعلم (خالد) طلابه إلى الأقسام الآتية: سمعي، بصري، حسي؛ اعتمد المعلم في تقسيمه طلابه على:",
            "options": ["الذكاءات المتعددة", "أنماط الشخصية", "نظريات التعلم", "أنماط التعلم"],
            "answer": 3,
            "explanations": {
                "correct": "أنماط التعلم تشير إلى الطريقة التي يفضلها الطالب لاستيعاب المعلومات: سمعي، بصري، حسي.",
                "wrong1": "الذكاءات المتعددة تشمل القدرات المختلفة وليس تقسيمًا حسب أسلوب التعلم فقط.",
                "wrong2": "أنماط الشخصية تتعلق بالسلوكيات والسمات الشخصية، لا بأسلوب التعلم فقط.",
                "wrong3": "نظريات التعلم تشير إلى النظريات التربوية العامة."
            }
        },
        {
            "id": 51,
            "q": "يسعى المعلم (فهد) إلى تطوير خططه التدريسية باستمرار، ويفكر دائمًا في دروسه وما يحتاج إلى تعديل؛ أنسب ممارسة يجب أن يستخدمها لتطوير خططه التدريسية:",
            "options": ["تطبيق الاستراتيجيات الحديثة في التقويم", "استخدام أحدث التقنيات التعليمية", "التنوع في استخدام طرق التدريس", "الاستفادة من نتائج التقويم"],
            "answer": 3,
            "explanations": {
                "correct": "الاستفادة من نتائج التقويم تساعد المعلم على تعديل وتحسين خططه التدريسية بشكل مستمر.",
                "wrong1": "تطبيق الاستراتيجيات الحديثة مفيد لكنه غير كافٍ بمفرده.",
                "wrong2": "استخدام أحدث التقنيات مفيد، لكنه لا يعكس تطوير مستمر بالتحليل.",
                "wrong3": "التنوع في طرق التدريس مفيد، لكنه لا يعكس استخدام التغذية الراجعة لتحسين الخطط."
            }
        },
        {
            "id": 52,
            "q": "طبق معلم اختبارًا على 50 طالبًا، فأجاب 30 منهم على السؤال الأول إجابة صحيحة؛ ما معامل صعوبة هذا السؤال؟",
            "options": ["0.20", "0.30", "0.40", "0.60"],
            "answer": 3,
            "explanations": {
                "correct": "معامل الصعوبة = عدد الإجابات الصحيحة ÷ إجمالي الطلاب = 30 ÷ 50 = 0.6.",
                "wrong1": "0.20: حساب خاطئ.",
                "wrong2": "0.30: حساب خاطئ.",
                "wrong3": "0.40: حساب خاطئ."
            }
        },
        {
            "id": 53,
            "q": "أنسب مخطط يوضح التشتت بين متغيرين:",
            "options": ["الانتشار", "الانحدار", "المنحنى", "المضلع التكراري"],
            "answer": 0,
            "explanations": {
                "correct": "مخطط الانتشار (Scatter plot) يوضح العلاقة والتشتت بين متغيرين.",
                "wrong1": "الانحدار يستخدم للتنبؤ بالاتجاه وليس لرصد التشتت فقط.",
                "wrong2": "المنحنى يوضح تغير متغير واحد مع الزمن عادة.",
                "wrong3": "المضلع التكراري يوضح تكرار البيانات لمتغير واحد."
            }
        },
        {
            "id": 54,
            "q": "ترتكز المعايير المهنية لرتب المعلمين على ثلاث مجالات مترابطة:",
            "options": ["القيم – المعرفة – الممارسة", "الأمانة – العطاء – الالتزام", "التدريب – القدرة – المهارة", "التخطيط – الأداء – التطوير"],
            "answer": 0,
            "explanations": {
                "correct": "المجالات الثلاثة الأساسية هي: القيم الأخلاقية، المعرفة المهنية، والممارسة العملية.",
                "wrong1": "الأمانة والعطاء والالتزام صفات مرغوبة لكنها ليست التصنيف المهني الرسمي.",
                "wrong2": "التدريب والقدرة والمهارة أدوات، وليست مجالات تقييم.",
                "wrong3": "التخطيط والأداء والتطوير خطوات عملية، لا مجالات تقييمية."
            }
        },
        {
            "id": 55,
            "q": "التعزيز السلبي يستخدمه دائمًا المعلم في الموقف التعليمي لـ:",
            "options": ["تقوية السلوك", "إضعاف السلوك", "المحافظة على السلوك", "إطفاء السلوك"],
            "answer": 0,
            "explanations": {
                "correct": "التعزيز السلبي يقوي السلوك عن طريق إزالة موقف مزعج عند أداء السلوك المطلوب.",
                "wrong1": "إضعاف السلوك: هذا دور العقاب.",
                "wrong2": "المحافظة على السلوك: غير دقيق، التعزيز يهدف للتقوية.",
                "wrong3": "إطفاء السلوك: يشير لإزالة الاستجابة عند عدم التعزيز."
            }
        },
        {
            "id": 56,
            "q": "صمم معلم برنامجًا حاسوبيًا مفتوحًا يضم أسئلة اختيار من متعدد، مع تعزيز بوجه ضاحك عند الإجابة الصحيحة ومحاولات أخرى عند الخطأ؛ هذا البرنامج مصمم وفق المدخل:",
            "options": ["الاجتماعي", "الإنساني", "السلوكي", "المعرفي"],
            "answer": 2,
            "explanations": {
                "correct": "المدخل السلوكي يركز على التعزيز والمكافأة لتقوية السلوك المرغوب.",
                "wrong1": "الاجتماعي: يركز على التفاعل بين الأفراد.",
                "wrong2": "الإنساني: يركز على القيم والذات والاحتياجات.",
                "wrong3": "المعرفي: يركز على العمليات العقلية وفهم المعلومات."
            }
        },
        {
            "id": 57,
            "q": "صمم معلم خطة تقويم تهدف إلى الكشف عن صعوبات التعلم، وتقديم تغذية راجعة، ووضع حلول لمعالجة الصعوبات؛ ما نوع التقويم المتبع؟",
            "options": ["التشخيصي", "البنائي (التكويني)", "الختامي", "المعياري"],
            "answer": 1,
            "explanations": {
                "correct": "التقويم البنائي أو التكويني يركز على التغذية الراجعة لتحسين التعلم وتحديد الصعوبات أثناء العملية التعليمية.",
                "wrong1": "التقويم التشخيصي يركز على تحديد المشكلات قبل بدء التعلم.",
                "wrong2": "التقويم الختامي يقيم بعد انتهاء التعلم فقط.",
                "wrong3": "التقويم المعياري يقارن الطلاب بمعيار محدد وليس لتحسين التعلم الفردي."
            }
        },
        {
            "id": 58,
            "q": "فن تعبيري يعد إعداده تدريبًا على الكتابة ومعرفة الأفكار الرئيسة:",
            "options": ["التقرير", "الرسالة", "المحضر", "التلخيص"],
            "answer": 3,
            "explanations": {
                "correct": "التلخيص يساعد الطلاب على استخراج الأفكار الرئيسية وإعادة صياغتها بطريقة مختصرة.",
                "wrong1": "التقرير يحتوي على تفاصيل كاملة وليست مختصرة فقط.",
                "wrong2": "الرسالة وسيلة تواصل وليست تدريبًا على استخراج الأفكار.",
                "wrong3": "المحضر يركز على توثيق الاجتماعات وليس التلخيص الأدبي."
            }
        },
        {
            "id": 59,
            "q": "عندما يجيب الطالب إجابات صحيحة عديدة دون تلقي أي تعزيز من المعلم قد يؤدي ذلك إلى التراخي من المشاركة لاحقًا، ويسمى هذا مبدأ الانطفاء في نظرية:",
            "options": ["الجشطلت", "النمو المعرفي", "التعلم الشرطي", "التعلم الإجرائي"],
            "answer": 3,
            "explanations": {
                "correct": "التعلم الإجرائي يوضح مبدأ الانطفاء عندما لا يُعزز السلوك الصحيح، فيتلاشى تدريجيًا.",
                "wrong1": "الجشطلت يركز على الإدراك الكلي والتصورات.",
                "wrong2": "النمو المعرفي يركز على التطور العقلي للطفل.",
                "wrong3": "التعلم الشرطي الكلاسيكي مختلف، يعتمد على الربط بين المنبه والاستجابة."
            }
        },
        {
            "id": 60,
            "q": "شرح المعلم لطلابه طريقة إعداد تقارير أدائهم مستعينًا بتحديد مستوى كل طالب بناءً على أداء زملائه؛ أي أنواع المراجع يعتمد في إعداد التقارير؟",
            "options": ["ذاتي المرجع", "محكي المرجع", "قياسي المرجع", "معياري المرجع"],
            "answer": 3,
            "explanations": {
                "correct": "المعياري المرجع يقارن أداء الطالب مع أداء مجموعة محددة (زملائه) لتحديد مستواه.",
                "wrong1": "ذاتي المرجع: يعتمد على تقييم الطالب لنفسه فقط.",
                "wrong2": "محكي المرجع: يعتمد على خبرة المعلم دون مقارنة بالآخرين.",
                "wrong3": "قياسي المرجع: يعتمد على معيار محدد ثابت، وليس مقارنة بالزملاء."
            }
        },
        {
            "id": 61,
            "q": "سامي طالب بالصف الأول الابتدائي أصبح قادرًا على إدراك أن العملية 6×2×4 هي نفسها 4×2×6؛ في أي مرحلة من مراحل النمو عند بياجيه يكون؟",
            "options": ["الحسية الحركية", "العمليات المادية (العيانية)", "ما قبل العمليات", "العمليات المجردة"],
            "answer": 1,
            "explanations": {
                "correct": "مرحلة العمليات المادية (العيانية) تتيح للطفل إدراك التعادل بين العمليات وفهم العلاقات المنطقية بين الأعداد.",
                "wrong1": "الحسية الحركية: التركيز على الحركة والحواس وليس العمليات العددية.",
                "wrong2": "ما قبل العمليات: تفكير محدود بالتمثيلات الرمزية فقط.",
                "wrong3": "العمليات المجردة: تفكير منطقي على الأفكار المجردة وليس الأشياء المادية المباشرة."
            }
        },
        {
            "id": 62,
            "q": "الخصائص الآتية تنطبق على النص الحجاجي (الجدلي) ما عدا:",
            "options": ["يعرض الأفكار بصورة سلسة مباشرة", "يهتم بأساليب الموازنة والمقابلة", "يكتب بلغة تقريرية موضوعية", "يهتم بالخيال وإثارة الدهشة"],
            "answer": 3,
            "explanations": {
                "correct": "النص الحجاجي يركز على تقديم الحجج ومقارنة الآراء وليس إثارة الخيال.",
                "wrong1": "يعرض الأفكار بصورة سلسة: صحيح ويميز النص الجدلي.",
                "wrong2": "يهتم بأساليب الموازنة: جزء من الخصائص الحجاجية.",
                "wrong3": "يكتب بلغة تقريرية: صحيح، توجيه المعلومات بشكل موضوعي."
            }
        },
        {
            "id": 63,
            "q": "من صفات البيئة الصفية الداعمة للتعلم الاجتماعي الانفعالي:",
            "options": ["تحدي القدرات", "العمل بروح الفريق", "المساواة بين الطلاب", "التنافسية بين الطلاب"],
            "answer": 1,
            "explanations": {
                "correct": "العمل بروح الفريق يعزز التعلم الاجتماعي الانفعالي ويشجع التعاون بين الطلاب.",
                "wrong1": "تحدي القدرات: مهم لكن لا يعكس جانب التعلم الاجتماعي الانفعالي.",
                "wrong2": "المساواة: صفة عامة وليست خاصة بالجانب الاجتماعي الانفعالي.",
                "wrong3": "التنافسية: قد تؤثر سلبًا على التعلم الاجتماعي الانفعالي."
            }
        },
        {
            "id": 64,
            "q": "من صور التفاعل الإيجابي الذي يقوم به المعلم مع أولياء الأمور استخدام تقنيات التواصل لاطلاعهم على:",
            "options": ["أهداف المقررات الدراسية", "الأهداف المعرفية ذات الأولوية", "خططه التدريسية وتعلم الطلاب", "تنظيم العمل التعليمي والإرشادي"],
            "answer": 2,
            "explanations": {
                "correct": "التواصل مع أولياء الأمور حول خطط التدريس وتقدم التعلم يعزز الشراكة الفعالة.",
                "wrong1": "أهداف المقررات: مهمة لكنها عامة ولا تعكس متابعة أداء الطلاب.",
                "wrong2": "الأهداف المعرفية: محدودة مقارنة بالخطط التفصيلية.",
                "wrong3": "تنظيم العمل: يتعلق بالإدارة وليس التواصل التربوي."
            }
        },
        {
            "id": 65,
            "q": "أوجد الانحراف المعياري إذا علمت أن التباين 81:",
            "options": ["2", "3", "8", "9"],
            "answer": 3,
            "explanations": {
                "correct": "الانحراف المعياري = الجذر التربيعي للتباين = √81 = 9.",
                "wrong1": "2: خطأ في الحساب.",
                "wrong2": "3: خطأ في الجذر التربيعي.",
                "wrong3": "8: خطأ تقديري."
            }
        },
        {
            "id": 66,
            "q": "في مساء أحد الأيام صادفك أحد أولياء الأمور معبرًا عن استيائه من تعرض ابنه المتكرر للتنمر من قبل بعض زملائه؛ كيف تستجيب بأسلوب أفضل؟",
            "options": ["أوضح له أن المدرسة لا تمتلك الصلاحيات وأنصحه بالاتصال بالجهات المختصة", "أستمع للمشكلة ثم أخبره بمتابعة ذلك مع المرشد الطلابي في المدرسة", "أعتبر الأمر بسيطًا وأخبره أنه جزء طبيعي من الحياة المدرسية", "أخبره بضرورة مراجعة الإدارة لأن هذا الأمر ليس من طبيعة عملي"],
            "answer": 1,
            "explanations": {
                "correct": "أفضل أسلوب هو الاستماع والمتابعة مع المرشد الطلابي لضمان التعامل مع المشكلة بشكل تربوي مناسب.",
                "wrong1": "تجاهل دور المدرسة غير مهني.",
                "wrong2": "اعتبار التنمر جزء طبيعي خطأ تربوي.",
                "wrong3": "إحالة الإدارة فقط دون متابعة المشكلة غير فعال."
            }
        },
        {
            "id": 67,
            "q": "التأمل في الأداء المهني ومحاولة تبريره بطرح حل واحد يعكس أحد مستويات التأمل في عملية النمو المهني وهو:",
            "options": ["الناقد", "الوصفي", "الحواري", "التفسيري"],
            "answer": 1,
            "explanations": {
                "correct": "المستوى الوصفي يركز على وصف الأداء وطرح حل واحد لتحسينه.",
                "wrong1": "الناقد: تحليل نقدي متعدد للخيارات.",
                "wrong2": "الحواري: يشمل مناقشة وتبادل الآراء.",
                "wrong3": "التفسيري: يعالج تفسير النتائج بشكل أعمق."
            }
        },
        {
            "id": 68,
            "q": "في موقف تعليمي بدأ المعلم الحديث عن ظاهرة طبيعية ثم كلف الطلاب بتنفيذ تجارب ومناقشة النتائج للوصول إلى استنتاجات؛ أي استراتيجية يستخدم؟",
            "options": ["التعلم بالاكتشاف", "التلميذ التعاوني", "التعلم المباشر", "التعلم القائم على المشروعات"],
            "answer": 0,
            "explanations": {
                "correct": "التعلم بالاكتشاف يعتمد على قيام الطلاب بتجارب واستخلاص النتائج بأنفسهم.",
                "wrong1": "التعلم التعاوني: يركز على العمل الجماعي، لكنه لا يحدد التجربة والاكتشاف الفردي.",
                "wrong2": "التعلم المباشر: يعتمد على الشرح من المعلم فقط.",
                "wrong3": "التعلم القائم على المشروعات: يرتكز على مشروع طويل المدى وليس تجربة قصيرة."
            }
        }
    );
    
    // إعادة تهيئة المصفوفات
    userAnswers = Array(questions.length).fill(null);
    answerLocked = Array(questions.length).fill(false);
    
    // إعادة تحميل الاختبار
    loadQuiz();
    // تحديث قائمة الأسئلة إذا كانت ظاهرة
    if (document.getElementById('questions-overlay').style.display === 'block') {
        showQuestionsList();
    }
    
    // إظهار رسالة نجاح
    alert("تم تحميل جميع الأسئلة بنجاح! استعن بالله وابدأ الاختبار");
}

// بدء التحميل الأولي
window.onload = function() {
    checkDarkModePreference();
    loadQuiz();
    startTimer();
    updateWhatsappButton();
    
    // إضافة تأثيرات عند التحميل
    document.querySelector('.hero-section').classList.add('bounce-in');
    setTimeout(() => {
        document.querySelector('.card').classList.add('fade-in');
    }, 300);
}
</script>
</body>
</html>
