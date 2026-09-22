<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>祝福生成器</title>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }

        body {
            font-family: 'Microsoft YaHei', 'PingFang SC', sans-serif;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            padding: 20px;
        }

        .container {
            background: rgba(255, 255, 255, 0.95);
            border-radius: 20px;
            padding: 40px 30px;
            width: 100%;
            max-width: 480px;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
            text-align: center;
        }

        h1 { color: #5b21b6; font-size: 28px; margin-bottom: 10px; }

        .subtitle { color: #6b7280; margin-bottom: 30px; font-size: 14px; }

        .input-group { display: flex; gap: 10px; margin-bottom: 30px; }

        #nameInput {
            flex: 1;
            padding: 12px 16px;
            border: 2px solid #ddd6fe;
            border-radius: 12px;
            font-size: 16px;
            outline: none;
            transition: border-color 0.3s;
        }
        #nameInput:focus { border-color: #7c3aed; }

        #generateBtn {
            padding: 12px 20px;
            background: linear-gradient(135deg, #7c3aed 0%, #db2777 100%);
            color: white;
            border: none;
            border-radius: 12px;
            font-size: 16px;
            cursor: pointer;
            transition: transform 0.2s, box-shadow 0.2s;
        }
        #generateBtn:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 20px rgba(124, 58, 237, 0.4);
        }

        .blessing-box {
            background: linear-gradient(135deg, #fef3c7 0%, #fde68a 100%);
            border-radius: 16px;
            padding: 24px;
            margin-bottom: 20px;
            text-align: left;
            animation: fadeIn 0.6s ease;
        }
        .blessing-title { color: #92400e; font-size: 18px; font-weight: bold; margin-bottom: 12px; }
        #displayName { color: #b45309; }
        .blessing-text { color: #78350f; font-size: 16px; line-height: 1.8; margin-bottom: 16px; white-space: pre-line; }
        .blessing-sign { text-align: right; color: #a16207; font-size: 13px; font-style: italic; }

        .copy-btn {
            padding: 10px 24px;
            background: #10b981;
            color: white;
            border: none;
            border-radius: 10px;
            font-size: 14px;
            cursor: pointer;
            transition: background 0.2s;
        }
        .copy-btn:hover { background: #059669; }

        .hidden { display: none; }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to   { opacity: 1; transform: translateY(0); }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>✨ 专属祝福生成器</h1>
        <p class="subtitle">输入你的名字，收获一份温暖的祝福</p>

        <div class="input-group">
            <input type="text" id="nameInput" placeholder="请输入你的名字" maxlength="20">
            <button id="generateBtn">生成祝福</button>
        </div>

        <div id="blessingBox" class="blessing-box hidden">
            <div class="blessing-title">亲爱的 <span id="displayName"></span>：</div>
            <div id="blessingText" class="blessing-text"></div>
            <div class="blessing-sign" id="blessingSign"></div>
        </div>

        <button id="copyBtn" class="copy-btn hidden">复制祝福</button>
    </div>

    <script>
    (function () {
        var nameInput     = document.getElementById('nameInput');
        var generateBtn   = document.getElementById('generateBtn');
        var blessingBox   = document.getElementById('blessingBox');
        var displayName   = document.getElementById('displayName');
        var blessingText  = document.getElementById('blessingText');
        var blessingSign  = document.getElementById('blessingSign');
        var copyBtn       = document.getElementById('copyBtn');

        // 自动填入当天日期
        var today = new Date();
        var dateStr = today.getFullYear() + '-'
            + String(today.getMonth() + 1).padStart(2, '0') + '-'
            + String(today.getDate()).padStart(2, '0');
        blessingSign.textContent = '—— 来自 ' + dateStr + ' 的祝福';

        var templates = [
            '愿你在新的一天里，\n眼里有光，心中有爱，\n所行皆坦途，所遇皆温暖。',
            '愿你的生活像春天的花朵，\n绚烂多彩，芬芳四溢；\n愿你的未来像星辰大海，\n辽阔无垠，充满希望。',
            '愿你被世界温柔以待，\n愿你所有的努力都不被辜负，\n愿幸福和快乐永远围绕着你。',
            '愿你拥有披荆斩棘的勇气，\n也拥有被生活宠爱的幸运，\n前路浩浩荡荡，万事尽可期待。',
            '愿你心中有梦，眼里有光，\n脚下有路，未来可期；\n愿每一天都比昨天更灿烂。',
            '愿你的世界没有烦恼，\n愿你的笑容永远灿烂，\n愿所有的美好都如期而至。',
            '愿你像向日葵一样，\n永远向着阳光生长，\n积极向上，温暖明亮。',
            '愿你的人生如茶，\n初尝微苦，回味甘甜；\n愿你历经山河，仍觉人间值得。'
        ];

        function generateBlessing(name) {
            var hash = 0;
            for (var i = 0; i < name.length; i++) {
                hash += name.charCodeAt(i);
            }
            var tpl = templates[hash % templates.length];
            return '嘿，' + name + '！\n' + tpl + '\n\n愿「' + name + '」这个名字，\n成为你人生中最美的符号之一。';
        }

        function showBlessing() {
            var name = nameInput.value.trim();
            if (!name) { alert('请先输入你的名字哦~'); nameInput.focus(); return; }
            if (name.length > 20) { alert('名字太长啦，请输入20个字以内~'); return; }

            displayName.textContent = name;
            blessingText.textContent = generateBlessing(name);
            blessingBox.classList.remove('hidden');
            copyBtn.classList.remove('hidden');

            blessingBox.style.animation = 'none';
            blessingBox.offsetHeight;
            blessingBox.style.animation = 'fadeIn 0.6s ease';
        }

        generateBtn.addEventListener('click', showBlessing);
        nameInput.addEventListener('keypress', function (e) {
            if (e.key === 'Enter') showBlessing();
        });

        copyBtn.addEventListener('click', function () {
            var fullText = '亲爱的 ' + displayName.textContent + '：\n' + blessingText.textContent;
            if (navigator.clipboard) {
                navigator.clipboard.writeText(fullText).then(function () {
                    var old = copyBtn.textContent;
                    copyBtn.textContent = '已复制 ✓';
                    setTimeout(function () { copyBtn.textContent = old; }, 2000);
                }).catch(function () { alert('复制失败，请手动复制~'); });
            } else {
                alert('浏览器不支持自动复制，请手动复制~');
            }
        });
    })();
    </script>
</body>
</html>
