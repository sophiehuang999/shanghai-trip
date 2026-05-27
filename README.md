<!DOCTYPE html>
<html lang="zh-Hant">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>上海行｜Travel App</title>

  <!-- Tailwind -->
  <script src="https://cdn.tailwindcss.com"></script>

  <!-- FontAwesome -->
  <link rel="stylesheet"
    href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css" />

  <!-- Google Fonts -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@500;700&family=Noto+Sans+TC:wght@300;400;500;700&display=swap" rel="stylesheet">

  <style>
    body {
      font-family: 'Noto Sans TC', sans-serif;
      background: #fffaf5;
      color: #5f4b45;
    }

    .title-font {
      font-family: 'Cormorant Garamond', serif;
    }

    .glass {
      background: rgba(255,255,255,0.8);
      backdrop-filter: blur(10px);
    }

    .soft-card {
      background: #fffdfb;
      border-radius: 28px;
      box-shadow:
        0 8px 30px rgba(221, 190, 169, 0.18);
    }

    .nav-btn.active {
      background: #f6d7cf;
      color: #7b5d55;
    }

    .timeline::before {
      content: "";
      position: absolute;
      left: 13px;
      top: 0;
      bottom: 0;
      width: 3px;
      background: #ead0c4;
    }

    .dot {
      width: 14px;
      height: 14px;
      background: #d7a98c;
      border-radius: 999px;
      position: absolute;
      left: 7px;
      top: 10px;
    }

    iframe {
      border-radius: 20px;
    }

    .cute-input {
      border-radius: 18px;
      border: 1px solid #edd9d0;
      background: #fff;
      padding: 12px;
      width: 100%;
    }

    .cute-btn {
      background: #e7b7a7;
      color: white;
      border-radius: 18px;
      padding: 10px 16px;
      transition: 0.2s;
    }

    .cute-btn:hover {
      background: #d89e8b;
    }

    .link-btn {
      display: inline-block;
      margin-top: 8px;
      background: #f5e0d8;
      color: #7b5d55;
      padding: 6px 12px;
      border-radius: 999px;
      font-size: 13px;
    }

    .bottom-space {
      height: 90px;
    }
  </style>
</head>

<body>

  <!-- HEADER -->
  <header class="sticky top-0 z-40 glass px-5 py-4 border-b border-[#f2dfd7]">
    <div class="flex items-center justify-between">
      <div>
        <h1 class="title-font text-4xl text-[#8c6659]">上海行</h1>
        <p class="text-sm text-[#9d7b70]">浪漫奶油風旅遊小工具</p>
      </div>

      <div class="text-right text-sm">
        <div>4/30 - 5/5</div>
        <div class="text-[#c28f7c]">Taipei ✈ Shanghai</div>
      </div>
    </div>
  </header>

  <!-- CONTENT -->
  <main class="p-4 pb-24 space-y-5">

    <!-- PLAN -->
    <section id="plan" class="tab-section">

      <!-- Flight -->
      <div class="soft-card p-5">
        <div class="flex items-center gap-3 mb-4">
          <i class="fa-solid fa-plane-departure text-[#d89e8b] text-xl"></i>
          <h2 class="title-font text-2xl">航班資訊</h2>
        </div>

        <div class="space-y-4 text-sm">
          <div class="bg-[#fff6f2] rounded-2xl p-4">
            <div class="font-bold mb-2">台北 ➜ 上海</div>
            <div>4/30 18:50 桃園機場 T2</div>
            <div>航班：MU5006</div>
          </div>

          <div class="bg-[#fff6f2] rounded-2xl p-4">
            <div class="font-bold mb-2">上海 ➜ 台北</div>
            <div>5/5 14:15 上海虹橋機場 T1</div>
            <div>航班：MU5097</div>
          </div>
        </div>
      </div>

      <!-- Hotel -->
      <div class="soft-card p-5">
        <div class="flex items-center gap-3 mb-4">
          <i class="fa-solid fa-hotel text-[#d89e8b]"></i>
          <h2 class="title-font text-2xl">住宿資訊</h2>
        </div>

        <p class="leading-7">
          蘇州市 崑山市 集善路萬科魅力花園 西區 5棟 34樓
        </p>

        <a target="_blank"
          href="https://maps.google.com/?q=蘇州市崑山市集善路萬科魅力花園"
          class="link-btn">
          <i class="fa-solid fa-map-location-dot mr-1"></i>
          Google Maps
        </a>
      </div>

      <!-- Timeline -->
      <div class="soft-card p-5">
        <div class="flex items-center gap-3 mb-5">
          <i class="fa-solid fa-route text-[#d89e8b]"></i>
          <h2 class="title-font text-2xl">每日行程</h2>
        </div>

        <div class="relative timeline pl-10 space-y-8">

          <!-- DAY 1 -->
          <div class="relative">
            <div class="dot"></div>

            <div class="bg-[#fff7f4] rounded-3xl p-4">
              <h3 class="font-bold text-lg mb-3">
                Day 1｜外灘＋南京東路＋陸家嘴夜景
              </h3>

              <ul class="space-y-2 text-sm leading-6">
                <li>• 南京東路步行街</li>
                <li>• 和平飯店</li>
                <li>• 外灘萬國建築群</li>
                <li>• 東方明珠</li>
                <li>• 上海中心大廈</li>
              </ul>

              <div class="flex flex-wrap gap-2 mt-4">
                <a target="_blank"
                  href="https://maps.google.com/?q=外灘"
                  class="link-btn">外灘地圖</a>

                <a target="_blank"
                  href="https://maps.google.com/?q=東方明珠"
                  class="link-btn">東方明珠</a>
              </div>

              <textarea
                class="cute-input mt-4 memo-input"
                data-key="memo-day1"
                placeholder="行程備忘錄..."></textarea>

              <div class="memo-preview mt-2"></div>
            </div>
          </div>

          <!-- DAY 2 -->
          <div class="relative">
            <div class="dot"></div>

            <div class="bg-[#fff7f4] rounded-3xl p-4">
              <h3 class="font-bold text-lg mb-3">
                Day 2｜法租界文青散步日
              </h3>

              <ul class="space-y-2 text-sm leading-6">
                <li>• 武康路</li>
                <li>• 安福路</li>
                <li>• 衡山路</li>
                <li>• 新天地</li>
              </ul>

              <div class="flex flex-wrap gap-2 mt-4">
                <a target="_blank"
                  href="https://maps.google.com/?q=武康路"
                  class="link-btn">武康路</a>

                <a target="_blank"
                  href="https://maps.google.com/?q=新天地 上海"
                  class="link-btn">新天地</a>
              </div>

              <textarea
                class="cute-input mt-4 memo-input"
                data-key="memo-day2"
                placeholder="行程備忘錄..."></textarea>

              <div class="memo-preview mt-2"></div>
            </div>
          </div>

          <!-- DAY 3 -->
          <div class="relative">
            <div class="dot"></div>

            <div class="bg-[#fff7f4] rounded-3xl p-4">
              <h3 class="font-bold text-lg mb-3">
                Day 3｜上海迪士尼
              </h3>

              <ul class="space-y-2 text-sm leading-6">
                <li>• 創極速光輪</li>
                <li>• 加勒比海盜</li>
                <li>• 瘋狂動物城</li>
              </ul>

              <a target="_blank"
                href="https://maps.google.com/?q=上海迪士尼"
                class="link-btn">
                迪士尼地圖
              </a>

              <textarea
                class="cute-input mt-4 memo-input"
                data-key="memo-day3"
                placeholder="行程備忘錄..."></textarea>

              <div class="memo-preview mt-2"></div>
            </div>
          </div>

          <!-- DAY 4 -->
          <div class="relative">
            <div class="dot"></div>

            <div class="bg-[#fff7f4] rounded-3xl p-4">
              <h3 class="font-bold text-lg mb-3">
                Day 4｜朱家角 or 豫園
              </h3>

              <ul class="space-y-2 text-sm leading-6">
                <li>• 朱家角古鎮</li>
                <li>• 豫園</li>
                <li>• 城隍廟</li>
              </ul>

              <div class="flex flex-wrap gap-2 mt-4">
                <a target="_blank"
                  href="https://maps.google.com/?q=朱家角"
                  class="link-btn">朱家角</a>

                <a target="_blank"
                  href="https://maps.google.com/?q=豫園"
                  class="link-btn">豫園</a>
              </div>

              <textarea
                class="cute-input mt-4 memo-input"
                data-key="memo-day4"
                placeholder="行程備忘錄..."></textarea>

              <div class="memo-preview mt-2"></div>
            </div>
          </div>

          <!-- DAY 5 -->
          <div class="relative">
            <div class="dot"></div>

            <div class="bg-[#fff7f4] rounded-3xl p-4">
              <h3 class="font-bold text-lg mb-3">
                Day 5｜購物＋返程
              </h3>

              <ul class="space-y-2 text-sm leading-6">
                <li>• TX 淮海</li>
                <li>• IAPM</li>
                <li>• 靜安嘉里中心</li>
              </ul>

              <textarea
                class="cute-input mt-4 memo-input"
                data-key="memo-day5"
                placeholder="行程備忘錄..."></textarea>

              <div class="memo-preview mt-2"></div>
            </div>
          </div>

        </div>
      </div>
    </section>

    <!-- GUIDE -->
    <section id="guide" class="tab-section hidden space-y-5">

      <div class="soft-card p-5">
        <h2 class="title-font text-3xl mb-4">深度導覽</h2>

        <div class="space-y-8 leading-8">

          <div>
            <h3 class="text-xl font-bold mb-3">外灘 Bund</h3>

            <p>
              外灘是上海最具代表性的地標，19世紀時為租界區，
              聚集了英、美、法等國的銀行與洋行，
              因此形成現在著名的「萬國建築群」。
              夜晚燈光點亮後，可以同時看到歷史建築與陸家嘴現代天際線，
              被稱為「上海最浪漫的夜景」。
            </p>
          </div>

          <iframe
            class="w-full h-64"
            src="https://www.openstreetmap.org/export/embed.html?bbox=121.48%2C31.23%2C121.50%2C31.25&layer=mapnik">
          </iframe>

          <div>
            <h3 class="text-xl font-bold mb-3">武康路</h3>

            <p>
              武康路被譽為上海最美街道之一，
              沿路充滿法式洋房、梧桐樹與咖啡店。
              著名的「武康大樓」建於1924年，
              外觀像一艘巨型郵輪，也是上海熱門打卡地標。
            </p>
          </div>

          <iframe
            class="w-full h-64"
            src="https://www.openstreetmap.org/export/embed.html?bbox=121.43%2C31.20%2C121.45%2C31.22&layer=mapnik">
          </iframe>

          <div>
            <h3 class="text-xl font-bold mb-3">上海迪士尼</h3>

            <p>
              上海迪士尼是中國第一座迪士尼樂園，
              擁有全球首座「瘋狂動物城」園區。
              創極速光輪是園區最熱門設施之一，
              夜晚的煙火與城堡燈光秀非常值得欣賞。
            </p>
          </div>

        </div>
      </div>

    </section>

    <!-- WALLET -->
    <section id="wallet" class="tab-section hidden space-y-5">

      <!-- Exchange -->
      <div class="soft-card p-5">
        <h2 class="title-font text-3xl mb-5">匯率換算</h2>

        <div class="space-y-4">

          <div>
            <label class="text-sm">人民幣匯率 (1 RMB = ? TWD)</label>
            <input id="rateInput" class="cute-input" value="4.5">
          </div>

          <div>
            <label class="text-sm">輸入算式</label>
            <input id="calcInput"
              class="cute-input"
              placeholder="例如：500+200*3">
          </div>

          <button onclick="calculateExchange()" class="cute-btn w-full">
            計算
          </button>

          <div id="calcResult"
            class="bg-[#fff6f2] rounded-2xl p-4 text-center text-lg">
            -
          </div>
        </div>
      </div>

      <!-- Accounting -->
      <div class="soft-card p-5">
        <h2 class="title-font text-3xl mb-5">旅遊記帳</h2>

        <div class="space-y-4">

          <input id="expenseName"
            class="cute-input"
            placeholder="品項">

          <input id="expenseAmount"
            type="number"
            class="cute-input"
            placeholder="人民幣金額">

          <input
            type="file"
            accept="image/*"
            capture="environment"
            id="expensePhoto"
            class="cute-input">

          <button onclick="addExpense()" class="cute-btn w-full">
            新增記帳
          </button>
        </div>

        <div id="expenseList" class="mt-6 space-y-4"></div>
      </div>
    </section>

    <!-- LISTS -->
    <section id="lists" class="tab-section hidden space-y-5">

      <!-- Checklist -->
      <div class="soft-card p-5">
        <h2 class="title-font text-3xl mb-5">行前 CheckList</h2>

        <div id="checklist" class="space-y-3"></div>
      </div>

      <!-- Notes -->
      <div class="soft-card p-5">
        <h2 class="title-font text-3xl mb-5">個人備忘錄</h2>

        <textarea id="generalMemo"
          class="cute-input h-40"
          placeholder="輸入備忘錄或網址..."></textarea>

        <div id="generalMemoPreview" class="mt-4"></div>
      </div>
    </section>

    <!-- INFO -->
    <section id="info" class="tab-section hidden space-y-5">

      <div class="soft-card p-5">
        <h2 class="title-font text-3xl mb-5">旅遊資訊</h2>

        <div class="space-y-6">

          <div>
            <h3 class="font-bold mb-2">天氣預報</h3>

            <a target="_blank"
              href="https://weather.com/zh-TW/weather/today/l/Shanghai+China"
              class="link-btn">
              上海天氣
            </a>
          </div>

          <div>
            <h3 class="font-bold mb-2">緊急聯絡</h3>

            <ul class="space-y-2 text-sm leading-7">
              <li>🚓 警察：110</li>
              <li>🚑 救護車：120</li>
              <li>🔥 火警：119</li>
              <li>🇹🇼 台灣辦事處：021-6295-5000</li>
            </ul>
          </div>

          <div>
            <h3 class="font-bold mb-2">注意事項</h3>

            <ul class="space-y-2 text-sm leading-7">
              <li>• 行動支付為主，建議綁定支付寶。</li>
              <li>• 勿攜帶違禁食品與肉類入境。</li>
              <li>• 地鐵安檢較嚴格，避免攜帶危險物品。</li>
              <li>• 熱門景點假日人潮很多，建議早出發。</li>
            </ul>
          </div>

        </div>
      </div>

    </section>

    <div class="bottom-space"></div>

  </main>

  <!-- NAV -->
  <nav class="fixed bottom-0 left-0 right-0 glass border-t border-[#f0ddd5] px-2 py-2 z-50">
    <div class="grid grid-cols-5 gap-2">

      <button class="nav-btn active rounded-2xl py-2 text-sm"
        onclick="showTab('plan', this)">
        <i class="fa-solid fa-calendar-days block mb-1"></i>
        PLAN
      </button>

      <button class="nav-btn rounded-2xl py-2 text-sm"
        onclick="showTab('guide', this)">
        <i class="fa-solid fa-book-open block mb-1"></i>
        GUIDE
      </button>

      <button class="nav-btn rounded-2xl py-2 text-sm"
        onclick="showTab('wallet', this)">
        <i class="fa-solid fa-wallet block mb-1"></i>
        WALLET
      </button>

      <button class="nav-btn rounded-2xl py-2 text-sm"
        onclick="showTab('lists', this)">
        <i class="fa-solid fa-list-check block mb-1"></i>
        LISTS
      </button>

      <button class="nav-btn rounded-2xl py-2 text-sm"
        onclick="showTab('info', this)">
        <i class="fa-solid fa-circle-info block mb-1"></i>
        INFO
      </button>

    </div>
  </nav>

  <script>

    // TAB
    function showTab(id, btn) {
      document.querySelectorAll('.tab-section')
        .forEach(el => el.classList.add('hidden'));

      document.getElementById(id)
        .classList.remove('hidden');

      document.querySelectorAll('.nav-btn')
        .forEach(el => el.classList.remove('active'));

      btn.classList.add('active');
    }

    // MEMO
    document.querySelectorAll('.memo-input').forEach(input => {

      const key = input.dataset.key;
      const preview = input.nextElementSibling;

      input.value = localStorage.getItem(key) || '';

      renderMemo(preview, input.value);

      input.addEventListener('input', () => {
        localStorage.setItem(key, input.value);
        renderMemo(preview, input.value);
      });
    });

    function renderMemo(container, text) {

      const urlRegex = /(https?:\/\/[^\s]+)/g;

      container.innerHTML = text.replace(urlRegex, url => {
        return `
          <a href="${url}" target="_blank"
            class="link-btn">
            開啟連結
          </a>
        `;
      });
    }

    // CHECKLIST
    const checklistItems = [
      '旅遊平安不便險投保',
      '護照',
      '信用卡',
      '外幣',
      '行動電源',
      '相機',
      '充電線',
      '藥品',
      '防曬乳',
      '雨傘',
      '拖鞋',
      '眼罩',
      '尿布',
      '濕紙巾',
      '耳溫槍'
    ];

    const checklistDiv = document.getElementById('checklist');

    checklistItems.forEach(item => {

      const checked = localStorage.getItem('check_' + item) === 'true';

      const row = document.createElement('label');

      row.className =
        'flex items-center gap-3 bg-[#fff6f2] rounded-2xl p-3';

      row.innerHTML = `
        <input type="checkbox"
          ${checked ? 'checked' : ''}
          class="w-5 h-5">

        <span>${item}</span>
      `;

      const checkbox = row.querySelector('input');

      checkbox.addEventListener('change', () => {
        localStorage.setItem('check_' + item, checkbox.checked);
      });

      checklistDiv.appendChild(row);
    });

    // GENERAL MEMO
    const generalMemo = document.getElementById('generalMemo');
    const generalPreview = document.getElementById('generalMemoPreview');

    generalMemo.value = localStorage.getItem('generalMemo') || '';

    renderMemo(generalPreview, generalMemo.value);

    generalMemo.addEventListener('input', () => {
      localStorage.setItem('generalMemo', generalMemo.value);
      renderMemo(generalPreview, generalMemo.value);
    });

    // EXCHANGE
    function calculateExchange() {

      try {

        const rate = parseFloat(
          document.getElementById('rateInput').value
        );

        const expr =
          document.getElementById('calcInput').value;

        const rmb = eval(expr);

        const twd = rmb * rate;

        document.getElementById('calcResult').innerHTML = `
          人民幣：¥ ${rmb.toFixed(2)}
          <br>
          台幣：約 NT$ ${twd.toFixed(2)}
        `;

      } catch {
        alert('算式錯誤');
      }
    }

    // ACCOUNTING
    let expenses =
      JSON.parse(localStorage.getItem('expenses') || '[]');

    renderExpenses();

    function addExpense() {

      const name =
        document.getElementById('expenseName').value;

      const amount =
        parseFloat(document.getElementById('expenseAmount').value);

      const photoInput =
        document.getElementById('expensePhoto');

      if (!name || !amount) {
        alert('請輸入資料');
        return;
      }

      const reader = new FileReader();

      if (photoInput.files[0]) {

        reader.onload = function(e) {

          compressImage(e.target.result, compressed => {

            saveExpense(name, amount, compressed);
          });
        };

        reader.readAsDataURL(photoInput.files[0]);

      } else {
        saveExpense(name, amount, '');
      }
    }

    function compressImage(src, callback) {

      const img = new Image();

      img.onload = function() {

        const canvas = document.createElement('canvas');

        const maxWidth = 400;

        const scale = maxWidth / img.width;

        canvas.width = maxWidth;
        canvas.height = img.height * scale;

        const ctx = canvas.getContext('2d');

        ctx.drawImage(img, 0, 0, canvas.width, canvas.height);

        callback(canvas.toDataURL('image/jpeg', 0.6));
      };

      img.src = src;
    }

    function saveExpense(name, amount, photo) {

      const rate =
        parseFloat(document.getElementById('rateInput').value || 4.5);

      const twd = amount * rate;

      expenses.unshift({
        name,
        amount,
        twd,
        photo
      });

      localStorage.setItem('expenses', JSON.stringify(expenses));

      renderExpenses();

      document.getElementById('expenseName').value = '';
      document.getElementById('expenseAmount').value = '';
      document.getElementById('expensePhoto').value = '';
    }

    function renderExpenses() {

      const list = document.getElementById('expenseList');

      list.innerHTML = '';

      expenses.forEach((item, index) => {

        const card = document.createElement('div');

        card.className =
          'bg-[#fff6f2] rounded-3xl p-4 flex gap-4 items-center';

        card.innerHTML = `

          ${item.photo ?
            `<img src="${item.photo}"
              class="w-20 h-20 rounded-2xl object-cover">`
            : ''
          }

          <div class="flex-1">
            <div class="font-bold">${item.name}</div>

            <div class="text-sm mt-1">
              ¥ ${item.amount}
            </div>

            <div class="text-sm text-[#b67c67]">
              NT$ ${item.twd.toFixed(0)}
            </div>
          </div>

          <button
            onclick="deleteExpense(${index})"
            class="text-red-400">
            <i class="fa-solid fa-trash"></i>
          </button>
        `;

        list.appendChild(card);
      });
    }

    function deleteExpense(index) {

      expenses.splice(index, 1);

      localStorage.setItem('expenses', JSON.stringify(expenses));

      renderExpenses();
    }

  </script>

</body>
</html>
