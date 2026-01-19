
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>心理學與生活 - 期末複習 (進階版)</title>
    <!-- React & ReactDOM -->
    <script src="https://unpkg.com/react@18/umd/react.development.js" crossorigin></script>
    <script src="https://unpkg.com/react-dom@18/umd/react-dom.development.js" crossorigin></script>
    <!-- Babel for JSX -->
    <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+TC:wght@300;400;500;700&display=swap" rel="stylesheet">
    <style>
        body { 
            font-family: 'Noto Sans TC', sans-serif; 
            background-color: #f9fafb; 
        }
        /* 卡片翻轉特效 CSS */
        .card-flip { 
            perspective: 1000px; 
        }
        .card-inner { 
            position: relative; 
            width: 100%; 
            height: 100%; 
            text-align: center; 
            transition: transform 0.6s; 
            transform-style: preserve-3d; 
        }
        .flipped .card-inner { 
            transform: rotateY(180deg); 
        }
        .card-front, .card-back { 
            position: absolute; 
            width: 100%; 
            height: 100%; 
            backface-visibility: hidden; 
            -webkit-backface-visibility: hidden; /* Safari */
            display: flex; 
            align-items: center; 
            justify-content: center; 
            border-radius: 1rem; 
            padding: 1.5rem; 
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06); 
        }
        .card-front { 
            background-color: #ffffff; 
            color: #1f2937; 
            border: 1px solid #e5e7eb;
        }
        .card-back { 
            background-color: #4f46e5; 
            color: white; 
            transform: rotateY(180deg); 
        }
    </style>
</head>
<body>
    <div id="root"></div>

    <script type="text/babel">
        const { useState, useEffect } = React;

        // --- 工具函式：洗牌演算法 ---
        function shuffleArray(array) {
            const newArray = [...array];
            for (let i = newArray.length - 1; i > 0; i--) {
                const j = Math.floor(Math.random() * (i + 1));
                [newArray[i], newArray[j]] = [newArray[j], newArray[i]];
            }
            return newArray;
        }

        // --- SVG Icons Components ---
        const IconBase = ({ children, className }) => (
            <svg 
                xmlns="http://www.w3.org/2000/svg" 
                width="24" 
                height="24" 
                viewBox="0 0 24 24" 
                fill="none" 
                stroke="currentColor" 
                strokeWidth="2" 
                strokeLinecap="round" 
                strokeLinejoin="round" 
                className={className}
            >
                {children}
            </svg>
        );

        const Icons = {
            BookOpen: ({ className }) => (
                <IconBase className={className}>
                    <path d="M2 3h6a4 4 0 0 1 4 4v14a3 3 0 0 0-3-3H2z"/><path d="M22 3h-6a4 4 0 0 0-4 4v14a3 3 0 0 1 3-3h7z"/>
                </IconBase>
            ),
            Brain: ({ className }) => (
                <IconBase className={className}>
                    <path d="M9.5 2A2.5 2.5 0 0 1 12 4.5v15a2.5 2.5 0 0 1-4.96.44 2.5 2.5 0 0 1-2.96-3.08 3 3 0 0 1-.34-5.58 2.5 2.5 0 0 1 1.32-4.24 2.5 2.5 0 0 1 1.98-3A2.5 2.5 0 0 1 9.5 2Z"/>
                    <path d="M14.5 2A2.5 2.5 0 0 0 12 4.5v15a2.5 2.5 0 0 0 4.96.44 2.5 2.5 0 0 0 2.96-3.08 3 3 0 0 0 .34-5.58 2.5 2.5 0 0 0-1.32-4.24 2.5 2.5 0 0 0-1.98-3A2.5 2.5 0 0 0 14.5 2Z"/>
                </IconBase>
            ),
            Activity: ({ className }) => (
                <IconBase className={className}>
                    <polyline points="22 12 18 12 15 21 9 3 6 12 2 12"/>
                </IconBase>
            ),
            Eye: ({ className }) => (
                <IconBase className={className}>
                    <path d="M2 12s3-7 10-7 10 7 10 7-3 7-10 7-10-7-10-7Z"/><circle cx="12" cy="12" r="3"/>
                </IconBase>
            ),
            Smile: ({ className }) => (
                <IconBase className={className}>
                    <circle cx="12" cy="12" r="10"/><path d="M8 14s1.5 2 4 2 4-2 4-2"/><line x1="9" y1="9" x2="9.01" y2="9"/><line x1="15" y1="9" x2="15.01" y2="9"/>
                </IconBase>
            ),
            AlertCircle: ({ className }) => (
                <IconBase className={className}>
                    <circle cx="12" cy="12" r="10"/><line x1="12" y1="8" x2="12" y2="12"/><line x1="12" y1="16" x2="12.01" y2="16"/>
                </IconBase>
            ),
            CheckCircle: ({ className }) => (
                <IconBase className={className}>
                    <path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"/><polyline points="22 4 12 14.01 9 11.01"/>
                </IconBase>
            ),
            XCircle: ({ className }) => (
                <IconBase className={className}>
                    <circle cx="12" cy="12" r="10"/><path d="m15 9-6 6"/><path d="m9 9 6 6"/>
                </IconBase>
            ),
            ArrowLeft: ({ className }) => (
                <IconBase className={className}>
                    <line x1="19" y1="12" x2="5" y2="12"/><polyline points="12 19 5 12 12 5"/>
                </IconBase>
            ),
            RefreshCw: ({ className }) => (
                <IconBase className={className}>
                    <path d="M3 12a9 9 0 0 1 9-9 9.75 9.75 0 0 1 6.74 2.74L21 8"/><path d="M21 3v5h-5"/><path d="M21 12a9 9 0 0 1-9 9 9.75 9.75 0 0 1-6.74-2.74L3 16"/><path d="M8 21H3v-5"/>
                </IconBase>
            ),
            User: ({ className }) => (
                <IconBase className={className}>
                    <path d="M19 21v-2a4 4 0 0 0-4-4H9a4 4 0 0 0-4 4v2"/><circle cx="12" cy="7" r="4"/>
                </IconBase>
            ),
            Shuffle: ({ className }) => (
                <IconBase className={className}>
                    <polyline points="16 3 21 3 21 8" /><line x1="4" y1="20" x2="21" y2="3" /><polyline points="21 16 21 21 16 21" /><line x1="15" y1="15" x2="21" y2="21" /><line x1="4" y1="4" x2="9" y2="9" />
                </IconBase>
            ),
             ArrowRight: ({ className }) => (
                <IconBase className={className}>
                     <line x1="5" y1="12" x2="19" y2="12" /><polyline points="12 5 19 12 12 19" />
                </IconBase>
            )
        };

        // --- 課程資料 ---
        const courseData = [
            {
                id: "ch1-intro",
                title: "第一章：導論與情緒",
                icon: "Smile",
                color: "bg-orange-100 text-orange-600",
                description: "心理學定義、五大學派與情緒發展",
                notes: [
                    { title: "心理學定義", content: "研究個體「行為」與「心理歷程」的科學。" },
                    { title: "五大主要學派", content: "1. 精神分析 (佛洛伊德): 潛意識、性、幼年經驗\n2. 行為學派 (華森): 刺激-反應 (S-R)、行為是學習來的\n3. 人本學派 (馬斯洛): 自我實現、人性本善\n4. 認知學派 (皮亞傑): 訊息處理、思考歷程\n5. 生理心理學: 神經傳導、腦部結構" },
                    { title: "基本情緒發展", content: "嬰兒出生即有情緒。0-3個月: 微笑、驚嚇；3個月: 生氣；18個月: 害羞、自尊。" }
                ],
                flashcards: [
                    { q: "心理學之父 (實驗心理學)", a: "馮特 (Wundt)" },
                    { q: "精神分析學派的創始人", a: "佛洛伊德 (Freud)" },
                    { q: "強調「自我實現」與「需求層次」的學派", a: "人本主義學派 (Maslow)" },
                    { q: "只研究可觀察行為，強調「刺激-反應」的學派", a: "行為學派 (Watson)" }
                ],
                quiz: [
                    { q: "下列何者不是心理學五大學派之一？", options: ["精神分析", "行為學派", "占星學派", "人本學派"], ans: 2 },
                    { q: "行為學派強調行為是如何產生的？", options: ["潛意識驅動", "學習而來", "天生遺傳", "靈魂賦予"], ans: 1 },
                    { q: "根據講義，幾個月大的嬰兒開始出現「害羞」的情緒？", options: ["3個月", "6個月", "12個月", "18個月"], ans: 3 }
                ]
            },
            {
                id: "ch3-perception",
                title: "第三章：感覺與知覺",
                icon: "Eye",
                color: "bg-blue-100 text-blue-600",
                description: "閾限、適應、知覺組織與錯覺圖形",
                notes: [
                    { title: "感覺 vs 知覺", content: "感覺 (Sensation): 器官接收刺激；知覺 (Perception): 大腦解釋訊息。" },
                    { title: "絕對閾限 (Absolute Threshold)", content: "能被偵測到的最小刺激強度 (例如：晴朗夜晚48公里外的燭光)。" },
                    { title: "感覺適應", content: "長期暴露在同一刺激下，敏感度降低 (例：入芝蘭之室，久而不聞其香)。" },
                    { title: "知覺特性", content: "1. 相對性 (圖形與背景可逆)\n2. 恆常性 (大小、形狀、顏色不變)\n3. 錯覺 (大腦錯誤解釋)" }
                ],
                flashcards: [
                    { q: "感覺適應 (Sensory Adaptation)", a: "對持續不變的刺激反應逐漸減弱的現象" },
                    { q: "圖形與背景 (Figure-Ground)", a: "知覺組織的基本原則，如「魯賓之杯」(人臉與杯子)" },
                    { q: "絕對閾限", a: "50%的機會能偵測到的最小刺激量" }
                ],
                quiz: [
                    { q: "「入芝蘭之室，久而不聞其香」是哪種現象？", options: ["感覺剝奪", "感覺適應", "絕對閾限", "知覺恆常性"], ans: 1 },
                    { q: "一張圖既可以看成鴨子，也可以看成兔子，這顯示了知覺的什麼特性？", options: ["深度知覺", "圖形與背景的可逆性", "大小恆常性", "顏色對比"], ans: 1 },
                    { q: "在靜室內可以聽到6公尺外手錶的滴答聲，這是指？", options: ["差異閾限", "絕對閾限", "感覺適應", "超感官知覺"], ans: 1 }
                ]
            },
            {
                id: "ch7-personality",
                title: "第七章：人格與特質",
                icon: "User",
                color: "bg-purple-100 text-purple-600",
                description: "佛洛伊德三我結構、自我防衛機轉、A型性格",
                notes: [
                    { title: "佛洛伊德人格結構", content: "1. 本我 (Id): 快樂原則，原始慾望。\n2. 自我 (Ego): 現實原則，調節者。\n3. 超我 (Superego): 道德原則，良心。" },
                    { title: "自我防衛機轉", content: "壓抑、投射(把錯誤推給別人)、合理化(酸葡萄)、反向作用(表現與內心相反)、退化(變回小孩行為)。" },
                    { title: "A型性格特徵", content: "急躁、求成心切、好爭勝、完美主義、時間緊迫感。容易有心血管疾病風險。" }
                ],
                flashcards: [
                    { q: "遵循「快樂原則」的人格結構", a: "本我 (Id)" },
                    { q: "遵循「道德原則」的人格結構", a: "超我 (Superego)" },
                    { q: "自己做錯事卻說是別人帶壞，這是哪種防衛機轉？", a: "投射作用 (Projection)" },
                    { q: "吃不到葡萄說葡萄酸", a: "合理化作用 (Rationalization)" }
                ],
                quiz: [
                    { q: "A型性格的人最容易罹患哪種身體疾病？", options: ["胃潰瘍", "心血管疾病", "氣喘", "皮膚過敏"], ans: 1 },
                    { q: "佛洛伊德認為，人格中的「執行長」，負責協調現實的是？", options: ["本我", "自我", "超我", "忘我"], ans: 1 },
                    { q: "面對壓力時表現出像小孩子一樣的哭鬧行為，是哪種防衛機轉？", options: ["壓抑", "昇華", "退化", "否認"], ans: 2 }
                ]
            },
            {
                id: "ch10-11-health",
                title: "第十/十一章：心理衛生",
                icon: "Brain",
                color: "bg-green-100 text-green-600",
                description: "心理健康標準、周哈里窗、常見精神疾病",
                notes: [
                    { title: "心理異常判斷標準", content: "1. 偏離社會常規\n2. 適應不良\n3. 長期自覺苦惱\n4. 違法行為" },
                    { title: "周哈里窗 (Johari Window)", content: "1. 開放我 (自知人知)\n2. 盲目我 (自不知人知)\n3. 隱藏我 (自知人不知)\n4. 未知我 (自不知人不知)" },
                    { title: "常見疾病", content: "憂鬱症 (情緒低落)、精神分裂症 (幻覺/妄想)、強迫症、焦慮症。" }
                ],
                flashcards: [
                    { q: "自己知道，別人也知道的區域", a: "開放我 (Open Self)" },
                    { q: "自己不知道，但別人知道 (如口頭禪)", a: "盲目我 (Blind Self)" },
                    { q: "對現實有不合理的知覺，如幻聽、妄想", a: "精神分裂症 (Schizophrenia)" }
                ],
                quiz: [
                    { q: "在周哈里窗中，自己心中有秘密不讓別人知道，屬於哪個區域？", options: ["開放我", "盲目我", "隱藏我", "未知我"], ans: 2 },
                    { q: "下列何者通常被視為心理健康的標準？", options: ["完全沒有情緒波動", "能了解並接納自己", "從不犯錯", "依賴他人做決定"], ans: 1 },
                    { q: "感覺到有人在跟蹤自己但實際沒有，這種「妄想」常見於？", options: ["強迫症", "精神分裂症", "飲食障礙", "憂鬱症"], ans: 1 }
                ]
            },
            {
                id: "ch13-stress",
                title: "第十三章：壓力與調適",
                icon: "Activity",
                color: "bg-red-100 text-red-600",
                description: "一般適應症候群 (GAS)、衝突類型",
                notes: [
                    { title: "一般適應症候群 (GAS)", content: "1. 警覺反應期 (Alarm): 腎上腺素分泌，準備戰鬥或逃跑。\n2. 抗拒期 (Resistance): 身體試圖適應壓力。\n3. 耗竭期 (Exhaustion): 資源耗盡，崩潰生病。" },
                    { title: "心理衝突類型", content: "1. 雙趨衝突: 兩個都想要 (魚與熊掌)。\n2. 雙避衝突: 兩個都不想要 (前有狼後有虎)。\n3. 趨避衝突: 既想要又怕受傷害 (想吃甜食怕胖)。" }
                ],
                flashcards: [
                    { q: "GAS 壓力理論的提出者", a: "Selye (席爾)" },
                    { q: "既想去玩又怕考試不及格", a: "趨避衝突" },
                    { q: "兩個討厭的工作必須選一個做", a: "雙避衝突" }
                ],
                quiz: [
                    { q: "壓力反應的最後一個階段，身體資源耗盡而生病，稱為什麼期？", options: ["警覺期", "抗拒期", "耗竭期", "恢復期"], ans: 2 },
                    { q: "「想吃美食又怕胖」屬於哪種衝突？", options: ["雙趨衝突", "雙避衝突", "趨避衝突", "多重趨避衝突"], ans: 2 },
                    { q: "面對壓力時，下列何者是比較健康的調適方式？", options: ["否認問題存在", "尋求社會支持與解決問題", "攻擊他人", "過度飲酒"], ans: 1 }
                ]
            }
        ];

        // --- 主程式組件 ---
        function Header({ setView }) {
            const BookIcon = Icons.BookOpen;
            return (
                <header className="bg-white shadow-sm sticky top-0 z-50">
                    <div className="max-w-4xl mx-auto px-4 py-4 flex justify-between items-center">
                        <div 
                            className="flex items-center space-x-2 cursor-pointer" 
                            onClick={() => setView('home')}
                        >
                            <div className="bg-indigo-600 p-2 rounded-lg">
                                <BookIcon className="text-white w-6 h-6" />
                            </div>
                            <div>
                                <h1 className="text-xl font-bold text-gray-800">心理學與生活</h1>
                                <p className="text-xs text-gray-500">期末複習小幫手</p>
                            </div>
                        </div>
                    </div>
                </header>
            );
        }

        function TopicCard({ topic, onSelect }) {
            const Icon = Icons[topic.icon];
            return (
                <div 
                    onClick={() => onSelect(topic)}
                    className="bg-white rounded-xl shadow-sm hover:shadow-md transition-all cursor-pointer border border-gray-100 overflow-hidden transform hover:-translate-y-1"
                >
                    <div className={`h-2 ${topic.color.split(' ')[0]}`}></div>
                    <div className="p-5">
                        <div className="flex items-center space-x-3 mb-3">
                            <div className={`p-2 rounded-lg ${topic.color}`}>
                                <Icon className="w-5 h-5" />
                            </div>
                            <h3 className="font-bold text-gray-800">{topic.title}</h3>
                        </div>
                        <p className="text-sm text-gray-500 line-clamp-2">{topic.description}</p>
                    </div>
                </div>
            );
        }

        function StudyView({ topic, onBack }) {
            const [activeTab, setActiveTab] = useState('notes');
            const ArrowLeftIcon = Icons.ArrowLeft;
            
            return (
                <div className="max-w-4xl mx-auto px-4 py-6">
                    <button 
                        onClick={onBack}
                        className="flex items-center text-gray-500 hover:text-indigo-600 mb-4 transition-colors"
                    >
                        <ArrowLeftIcon className="w-4 h-4 mr-1" />
                        返回目錄
                    </button>

                    <div className="bg-white rounded-2xl shadow-sm overflow-hidden mb-6">
                        <div className="p-6 border-b border-gray-100">
                            <h2 className="text-2xl font-bold text-gray-800 flex items-center">
                                {topic.title}
                            </h2>
                            <p className="text-gray-500 mt-1">{topic.description}</p>
                        </div>
                        
                        <div className="flex border-b border-gray-100">
                            {['notes', 'flashcards', 'quiz'].map((tab) => (
                                <button
                                    key={tab}
                                    onClick={() => setActiveTab(tab)}
                                    className={`flex-1 py-4 text-sm font-medium transition-colors relative ${
                                        activeTab === tab ? 'text-indigo-600' : 'text-gray-500 hover:text-gray-700'
                                    }`}
                                >
                                    {tab === 'notes' && '重點筆記'}
                                    {tab === 'flashcards' && '記憶翻牌'}
                                    {tab === 'quiz' && '自我測驗'}
                                    {activeTab === tab && (
                                        <div className="absolute bottom-0 left-0 w-full h-0.5 bg-indigo-600"></div>
                                    )}
                                </button>
                            ))}
                        </div>

                        <div className="p-6 bg-gray-50 min-h-[400px]">
                            {activeTab === 'notes' && <NotesView notes={topic.notes} />}
                            {activeTab === 'flashcards' && <FlashcardsView cards={topic.flashcards} />}
                            {activeTab === 'quiz' && <QuizView quiz={topic.quiz} />}
                        </div>
                    </div>
                </div>
            );
        }

        function NotesView({ notes }) {
            return (
                <div className="space-y-4">
                    {notes.map((note, idx) => (
                        <div key={idx} className="bg-white p-5 rounded-xl border border-gray-100 shadow-sm">
                            <h3 className="font-bold text-lg text-indigo-700 mb-2">{note.title}</h3>
                            <p className="text-gray-600 whitespace-pre-line leading-relaxed">{note.content}</p>
                        </div>
                    ))}
                    <div className="mt-8 text-center text-gray-400 text-sm">
                        - 筆記整理自上傳講義 -
                    </div>
                </div>
            );
        }

        function FlashcardsView({ cards }) {
            const [displayCards, setDisplayCards] = useState(cards);
            const [currentCard, setCurrentCard] = useState(0);
            const [isFlipped, setIsFlipped] = useState(false);
            const ArrowRightIcon = Icons.ArrowRight;
            const ShuffleIcon = Icons.Shuffle;

            useEffect(() => {
                setDisplayCards(cards);
                setCurrentCard(0);
                setIsFlipped(false);
            }, [cards]);

            const handleNext = () => {
                setIsFlipped(false);
                setTimeout(() => {
                    setCurrentCard((prev) => (prev + 1) % displayCards.length);
                }, 300);
            };

            const handleShuffle = () => {
                setIsFlipped(false);
                setTimeout(() => {
                    setDisplayCards(shuffleArray(cards));
                    setCurrentCard(0);
                }, 300);
            };

            return (
                <div className="flex flex-col items-center justify-center h-full space-y-6 py-10">
                    <div className="flex justify-between w-full max-w-md items-center">
                        <div className="text-gray-500 text-sm font-medium">
                            卡片 {currentCard + 1} / {displayCards.length}
                        </div>
                        <button 
                            onClick={handleShuffle}
                            className="text-xs flex items-center text-indigo-600 hover:text-indigo-800 bg-indigo-50 px-3 py-1 rounded-full transition-colors"
                        >
                            <ShuffleIcon className="w-3 h-3 mr-1" />
                            洗牌
                        </button>
                    </div>
                    
                    <div 
                        className={`relative w-full max-w-md h-64 cursor-pointer card-flip ${isFlipped ? 'flipped' : ''}`}
                        onClick={() => setIsFlipped(!isFlipped)}
                    >
                        <div className="card-inner">
                            <div className="card-front border-2 border-indigo-50">
                                <div>
                                    <p className="text-xs text-gray-400 uppercase tracking-wider mb-2">題目</p>
                                    <h3 className="text-xl font-bold text-gray-800">{displayCards[currentCard].q}</h3>
                                    <p className="text-xs text-gray-400 mt-4">(點擊翻看答案)</p>
                                </div>
                            </div>
                            <div className="card-back">
                                <div>
                                    <p className="text-xs text-indigo-200 uppercase tracking-wider mb-2">答案</p>
                                    <h3 className="text-xl font-bold text-white">{displayCards[currentCard].a}</h3>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div className="flex space-x-4">
                        <button 
                            onClick={handleNext}
                            className="flex items-center space-x-2 px-6 py-2 bg-indigo-600 text-white rounded-full hover:bg-indigo-700 transition-colors shadow-md"
                        >
                            <span className="ml-1">下一張</span>
                            <ArrowRightIcon className="w-4 h-4" />
                        </button>
                    </div>
                </div>
            );
        }

        function QuizView({ quiz }) {
            const [quizQuestions, setQuizQuestions] = useState([]);
            const [answers, setAnswers] = useState({});
            const [showResult, setShowResult] = useState(false);
            const ActivityIcon = Icons.Activity;
            const CheckIcon = Icons.CheckCircle;
            const XIcon = Icons.XCircle;
            const RefreshIcon = Icons.RefreshCw;

            useEffect(() => {
                setQuizQuestions(shuffleArray(quiz));
                setAnswers({});
                setShowResult(false);
            }, [quiz]);

            const handleSelect = (qIdx, optIdx) => {
                if (showResult) return;
                setAnswers(prev => ({...prev, [qIdx]: optIdx}));
            };

            const calculateScore = () => {
                let correct = 0;
                quizQuestions.forEach((q, idx) => {
                    if (answers[idx] === q.ans) correct++;
                });
                return correct;
            };

            const resetQuiz = () => {
                setQuizQuestions(shuffleArray(quiz));
                setAnswers({});
                setShowResult(false);
                window.scrollTo({ top: 0, behavior: 'smooth' });
            };

            if (quizQuestions.length === 0) return <div>準備題庫中...</div>;

            return (
                <div className="max-w-2xl mx-auto space-y-8">
                    {!showResult ? (
                        <div className="space-y-6">
                            <div className="bg-yellow-50 text-yellow-800 p-3 rounded-lg text-sm text-center mb-4">
                                💡 題目順序已隨機打亂，請仔細作答！
                            </div>
                            {quizQuestions.map((q, idx) => (
                                <div key={idx} className="bg-white p-6 rounded-xl border border-gray-100 shadow-sm">
                                    <h3 className="font-bold text-gray-800 mb-4 flex">
                                        <span className="bg-indigo-100 text-indigo-600 w-6 h-6 rounded-full flex items-center justify-center text-xs mr-3 flex-shrink-0 mt-0.5">{idx + 1}</span>
                                        {q.q}
                                    </h3>
                                    <div className="space-y-2 pl-9">
                                        {q.options.map((opt, optIdx) => (
                                            <button
                                                key={optIdx}
                                                onClick={() => handleSelect(idx, optIdx)}
                                                className={`w-full text-left p-3 rounded-lg border transition-all ${
                                                    answers[idx] === optIdx 
                                                    ? 'border-indigo-600 bg-indigo-50 text-indigo-700' 
                                                    : 'border-gray-200 hover:bg-gray-50'
                                                }`}
                                            >
                                                {opt}
                                            </button>
                                        ))}
                                    </div>
                                </div>
                            ))}
                            <button 
                                onClick={() => setShowResult(true)}
                                disabled={Object.keys(answers).length < quizQuestions.length}
                                className="w-full py-3 bg-indigo-600 text-white rounded-xl font-bold shadow-lg hover:bg-indigo-700 disabled:opacity-50 disabled:cursor-not-allowed transition-all"
                            >
                                提交答案
                            </button>
                        </div>
                    ) : (
                        <div className="text-center py-10">
                            <div className="inline-block p-4 rounded-full bg-green-100 mb-4">
                                <ActivityIcon className="w-12 h-12 text-green-600" />
                            </div>
                            <h2 className="text-3xl font-bold text-gray-800 mb-2">測驗結果</h2>
                            <p className="text-xl text-gray-600 mb-8">
                                答對 {calculateScore()} / {quizQuestions.length} 題
                            </p>
                            
                            <div className="space-y-4 text-left max-w-xl mx-auto mb-8">
                                {quizQuestions.map((q, idx) => (
                                    <div key={idx} className={`p-4 rounded-lg border ${answers[idx] === q.ans ? 'border-green-200 bg-green-50' : 'border-red-200 bg-red-50'}`}>
                                        <p className="font-bold text-gray-800 mb-1">{idx + 1}. {q.q}</p>
                                        <p className="text-sm">
                                            你的選擇: <span className="font-medium">{q.options[answers[idx]]}</span> 
                                            {answers[idx] === q.ans ? (
                                                <span className="inline-flex items-center ml-2 text-green-500">
                                                    <CheckIcon className="w-4 h-4 mr-1" /> 正確
                                                </span>
                                            ) : (
                                                <span className="inline-flex items-center ml-2 text-red-500">
                                                    <XIcon className="w-4 h-4 mr-1" /> (正確答案: {q.options[q.ans]})
                                                </span>
                                            )}
                                        </p>
                                    </div>
                                ))}
                            </div>

                            <button 
                                onClick={resetQuiz}
                                className="flex items-center justify-center w-full px-8 py-3 bg-gray-800 text-white rounded-xl font-bold hover:bg-gray-900 transition-all"
                            >
                                <RefreshIcon className="w-4 h-4 mr-2" />
                                重新測驗 (題目將再次洗牌)
                            </button>
                        </div>
                    )}
                </div>
            );
        }

        function App() {
            const [view, setView] = useState('home');
            const [selectedTopic, setSelectedTopic] = useState(null);
            const BookIcon = Icons.BookOpen;

            const handleSelectTopic = (topic) => {
                setSelectedTopic(topic);
                setView('study');
                window.scrollTo({ top: 0, behavior: 'smooth' });
            };

            return (
                <div className="min-h-screen pb-10">
                    <Header setView={setView} />
                    
                    <main className="pt-6">
                        {view === 'home' ? (
                            <div className="max-w-4xl mx-auto px-4">
                                <div className="mb-8 text-center py-10 bg-indigo-600 rounded-3xl text-white shadow-xl bg-[url('https://www.transparenttextures.com/patterns/cubes.png')] relative overflow-hidden">
                                    <div className="relative z-10">
                                        <h2 className="text-3xl font-bold mb-4">準備好複習心理學了嗎？</h2>
                                        <p className="text-indigo-100 max-w-xl mx-auto">
                                            選一個章節開始，透過重點筆記、翻卡與測驗來強化你的記憶。
                                        </p>
                                    </div>
                                    <div className="absolute top-0 left-0 w-full h-full bg-black opacity-10"></div>
                                </div>
                                
                                <h3 className="text-xl font-bold text-gray-800 mb-4 flex items-center">
                                    <BookIcon className="w-5 h-5 mr-2 text-indigo-600" />
                                    課程章節
                                </h3>
                                <div className="grid grid-cols-1 md:grid-cols-2 gap-4">
                                    {courseData.map(topic => (
                                        <TopicCard 
                                            key={topic.id} 
                                            topic={topic} 
                                            onSelect={handleSelectTopic} 
                                        />
                                    ))}
                                </div>
                                <div className="mt-8 text-center text-gray-400 text-sm">
                                    資料來源：課程 PDF 講義
                                </div>
                            </div>
                        ) : (
                            <StudyView 
                                topic={selectedTopic} 
                                onBack={() => setView('home')} 
                            />
                        )}
                    </main>
                </div>
            );
        }

        const root = ReactDOM.createRoot(document.getElementById('root'));
        root.render(<App />);
    </script>
</body>
</html>
