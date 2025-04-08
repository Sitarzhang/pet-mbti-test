<!DOCTYPE html>
<html>
<head>
    <title>宠物MBTI性格测试</title>
    <style>
        body { font-family: Arial, sans-serif; max-width: 800px; margin: 0 auto; padding: 20px; }
        .question { margin: 20px 0; padding: 15px; border: 1px solid #ddd; border-radius: 8px; }
        button { padding: 10px 20px; background: #4CAF50; color: white; border: none; border-radius: 4px; cursor: pointer; }
        button:hover { background: #45a049; }
        .result { display: none; margin-top: 30px; padding: 20px; background: #f8f9fa; border-radius: 8px; }
    </style>
</head>
<body>
    <h1>🐾 宠物16人格MBTI测试 🐾</h1>
    
    <form id="petTest">
        <!-- 维度1: E vs I -->
        <div class="question">
            <p>1. 家中来客人时，您的宠物：</p>
            <label><input type="radio" name="q1" value="E" required> A. 热情迎接，主动示好</label><br>
            <label><input type="radio" name="q1" value="I"> B. 躲藏起来，保持警惕</label>
        </div>
        <div class="question">
            <p>2. 散步时，您的宠物更倾向于：</p>
            <label><input type="radio" name="q2" value="E"> A. 自由探索，对新路线充满好奇</label><br>
            <label><input type="radio" name="q2" value="I"> B. 紧跟主人，观察主人动态</label>
        </div>
        <div class="question">
            <p>3. 独自在家时，您的宠物：</p>
            <label><input type="radio" name="q3" value="E"> A. 频繁寻找互动（如扒门、叫唤）</label><br>
            <label><input type="radio" name="q3" value="I"> B. 安静睡觉或发呆，不吵闹</label>
        </div>
        <div class="question">
            <p>4. 面对其他宠物时，您的宠物：</p>
            <label><input type="radio" name="q4" value="E"> A. 主动靠近，试图玩耍</label><br>
            <label><input type="radio" name="q4" value="I"> B. 保持距离，观察后再决定</label>
        </div>

        <!-- 维度2: S vs N -->
        <div class="question">
            <p>5. 面对陌生环境或新事物，您的宠物：</p>
            <label><input type="radio" name="q5" value="S"> A. 小心谨慎，逐步适应</label><br>
            <label><input type="radio" name="q5" value="N"> B. 兴奋好奇，立即尝试</label>
        </div>
        <div class="question">
            <p>6. 对食物的态度：</p>
            <label><input type="radio" name="q6" value="S"> A. 只吃熟悉的食物，拒绝新口味</label><br>
            <label><input type="radio" name="q6" value="N"> B. 愿意尝试新食物，甚至抢主人的零食</label>
        </div>
        <div class="question">
            <p>7. 同类相处时，您的宠物：</p>
            <label><input type="radio" name="q7" value="S"> A. 友好分享玩具或领地</label><br>
            <label><input type="radio" name="q7" value="N"> B. 争夺资源，展现“领导欲”</label>
        </div>
        <div class="question">
            <p>8. 探索新玩具时，您的宠物：</p>
            <label><input type="radio" name="q8" value="S"> A. 先嗅闻观察，再慢慢接触</label><br>
            <label><input type="radio" name="q8" value="N"> B. 直接扑上去撕咬或拍打</label>
        </div>

        <!-- 维度3: F vs T -->
        <div class="question">
            <p>9. 与主人互动时，您的宠物更喜欢：</p>
            <label><input type="radio" name="q9" value="F"> A. 安静陪伴，享受抚摸</label><br>
            <label><input type="radio" name="q9" value="T"> B. 追逐游戏或竞技类活动</label>
        </div>
        <div class="question">
            <p>10. 当您情绪低落时，您的宠物：</p>
            <label><input type="radio" name="q10" value="F"> A. 主动靠近安慰，表现黏人</label><br>
            <label><input type="radio" name="q10" value="T"> B. 无特殊反应，继续做自己的事</label>
        </div>
        <div class="question">
            <p>11. 面对其他宠物受伤时，您的宠物：</p>
            <label><input type="radio" name="q11" value="F"> A. 表现出关切，试图帮助</label><br>
            <label><input type="radio" name="q11" value="T"> B. 漠不关心，专注自己的活动</label>
        </div>
        <div class="question">
            <p>12. 被主人批评时的反应：</p>
            <label><input type="radio" name="q12" value="F"> A. 低头示弱或讨好</label><br>
            <label><input type="radio" name="q12" value="T"> B. 假装没听见，继续我行我素</label>
        </div>

        <!-- 维度4: J vs P -->
        <div class="question">
            <p>13. 日常作息规律：</p>
            <label><input type="radio" name="q13" value="J"> A. 定时吃饭、睡觉，习惯固定</label><br>
            <label><input type="radio" name="q13" value="P"> B. 随心情变化，作息不规律</label>
        </div>
        <div class="question">
            <p>14. 面对主人的指令：</p>
            <label><input type="radio" name="q14" value="J"> A. 严格遵守，执行力强</label><br>
            <label><input type="radio" name="q14" value="P"> B. 偶尔配合，更多按自己节奏行动</label>
        </div>
        <div class="question">
            <p>15. 整理毛发或窝垫的行为：</p>
            <label><input type="radio" name="q15" value="J"> A. 每天固定整理，保持整洁</label><br>
            <label><input type="radio" name="q15" value="P"> B. 随意躺卧，不太在意凌乱</label>
        </div>
        <div class="question">
            <p>16. 对新规则的适应速度：</p>
            <label><input type="radio" name="q16" value="J"> A. 快速接受并遵守</label><br>
            <label><input type="radio" name="q16" value="P"> B. 抗拒改变，需要时间适应</label>
        </div>

        <button type="button" onclick="calculateResult()">✨ 提交测试</button>
    </form>

    <div id="resultBox" class="result">
        <h2>测试结果：<span id="petType" style="color: #4CAF50;"></span></h2>
        <p id="typeDesc"></p>
    </div>

    <script>
        // 题目与维度的映射
        const questionDimensions = {
            q1: 'EI', q2: 'EI', q3: 'EI', q4: 'EI',
            q5: 'SN', q6: 'SN', q7: 'SN', q8: 'SN',
            q9: 'FT', q10: 'FT', q11: 'FT', q12: 'FT',
            q13: 'JP', q14: 'JP', q15: 'JP', q16: 'JP'
        };

        // 完整的16种性格描述
        const typeDescriptions = {
            "ISTJ": "🔒 守护者：可靠务实，严格遵守作息，喜欢规律的生活，讨厌意外变化。",
            "ISFJ": "🍼 照顾者：温柔贴心，默默记住主人的习惯，总是默默陪伴。",
            "INFJ": "🎭 哲学家：神秘敏锐，能感知主人的情绪，但保持自己的独立空间。",
            "INTJ": "🎯 战略家：独立冷静，喜欢制定自己的规则，对不感兴趣的事置之不理。",
            "ISTP": "🔧 手艺人：机智灵活，热衷探索新技能，比如自己开门或解锁玩具。",
            "ISFP": "🎨 艺术家：安静敏感，享受当下的小确幸，对陌生事物保持谨慎。",
            "INFP": "🌱 治愈者：理想主义，对世界充满好奇，容易对其他小动物产生同情。",
            "INTP": "🤔 思考者：高冷理性，喜欢观察和分析，对主人的呼唤选择性回应。",
            "ESTP": "⚡ 冒险家：精力旺盛，总能发现新乐趣！对新玩具充满征服欲。",
            "ESFP": "🎉 表演者：活泼热情，是家里的开心果，喜欢吸引所有人的注意。",
            "ENFP": "🌈 社交达人：热情好奇，喜欢互动和冒险，但对坚持训练缺乏耐心。",
            "ENTP": "💡 发明家：聪明狡黠，总能想出鬼点子，比如藏起主人的袜子来交换零食。",
            "ESTJ": "📋 管理者：强势果断，喜欢掌控环境，甚至会“管教”其他宠物。",
            "ESFJ": "👑 组织者：贴心周到，热衷社交互动，时刻关注家庭成员的动态。",
            "ENFJ": "🌟 导师型：善解人意，天生的小领导，会主动照顾新来的宠物。",
            "ENTJ": "🚀 指挥官：自信果断，喜欢发号施令，比如要求主人按时开饭。"
        };

        function calculateResult() {
            let scores = { E:0, I:0, S:0, N:0, F:0, T:0, J:0, P:0 };

            // 检查是否完成所有题目
            for (let q in questionDimensions) {
                const selected = document.querySelector(`input[name="${q}"]:checked`);
                if (!selected) {
                    alert("请先完成所有题目哦！");
                    return;
                }
                scores[selected.value] += 1;
            }

            // 计算最终类型
            const type = [
                scores.E >= scores.I ? 'E' : 'I',
                scores.S >= scores.N ? 'S' : 'N',
                scores.F >= scores.T ? 'F' : 'T',
                scores.J >= scores.P ? 'J' : 'P'
            ].join('');

            // 显示结果
            const resultBox = document.getElementById("resultBox");
            resultBox.style.display = "block";
            document.getElementById("petType").textContent = type;
            document.getElementById("typeDesc").textContent = typeDescriptions[type] || "您的宠物是神秘的存在！";
        }
    </script>
</body>
</html>
