<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
  <title>1830 맨체스터: 연기와 기계의 도시</title>
  <style>
    * { box-sizing: border-box; margin: 0; padding: 0; font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Noto Sans KR", sans-serif; }
    body { background-color: #1a1a1a; color: #e0e0e0; display: flex; justify-content: center; min-height: 100vh; }
    #app { width: 100%; max-width: 480px; background: #242424; min-height: 100vh; display: flex; flex-direction: column; padding: 20px; border-left: 1px solid #333; border-right: 1px solid #333; }
    h1 { font-size: 1.5rem; text-align: center; color: #e6b422; margin-bottom: 8px; line-height: 1.3; }
    h2 { font-size: 1.2rem; color: #fff; margin-bottom: 12px; }
    .subtitle { text-align: center; color: #999; font-size: 0.9rem; margin-bottom: 24px; }
    .card { background: #2f2f2f; border-radius: 8px; padding: 16px; margin-bottom: 16px; border: 1px solid #444; }
    .btn { width: 100%; background: #4a5568; color: #fff; border: none; padding: 14px 16px; border-radius: 8px; font-size: 1rem; cursor: pointer; margin-bottom: 10px; font-weight: 600; text-align: left; line-height: 1.4; transition: background 0.2s; }
    .btn:active { background: #2d3748; }
    .btn-primary { background: #b8860b; color: #fff; text-align: center; }
    .btn-primary:active { background: #996515; }
    .stats-bar { display: flex; justify-content: space-around; background: #1e1e1e; padding: 10px; border-radius: 8px; margin-bottom: 16px; border: 1px solid #3d3d3d; }
    .stat-item { text-align: center; font-size: 0.85rem; }
    .stat-value { font-weight: bold; font-size: 1.1rem; color: #e6b422; }
    .desc { font-size: 0.95rem; line-height: 1.6; color: #d1d5db; margin-bottom: 16px; word-break: keep-all; }
    .badge { display: inline-block; background: #7c2d12; color: #fed7aa; padding: 3px 8px; border-radius: 4px; font-size: 0.8rem; margin-bottom: 10px; font-weight: bold; }
    .hidden { display: none !important; }
    .feedback-box { background: #1f2937; border-left: 4px solid #3b82f6; padding: 12px; margin-bottom: 16px; font-size: 0.9rem; line-height: 1.5; color: #93c5fd; }
  </style>
</head>
<body>

<div id="app">
  <!-- 1. 시작 화면 -->
  <div id="screen-intro">
    <div style="text-align: center; margin-top: 20px; font-size: 3rem;">🏭</div>
    <h1>1830 맨체스터<br><span style="font-size: 1rem; color: #aaa;">연기와 기계의 도시</span></h1>
    <p class="subtitle">19세기 산업혁명 역사 체험 시뮬레이션</p>
    
    <div class="card desc">
      검은 연기가 하늘을 뒤덮은 1830년 영국 맨체스터.<br><br>
      증기기관과 기계가 인간의 손을 대신하기 시작하면서 엄청난 부가 축적되지만, 누군가는 하루 16시간 노동과 빈곤에 신음합니다.<br><br>
      당신은 이 격변의 시대에서 어떤 선택을 내리겠습니까?
    </div>

    <h2 style="font-size: 1rem; margin-top: 10px;">체험할 인물을 선택하세요:</h2>
    <button class="btn" onclick="startGame('tom')">👦 톰 (11세, 아동 노동자)<br><small style="color: #bbb; font-weight: normal;">방적기 아래 실 찌꺼기를 치우는 청소년</small></button>
    <button class="btn" onclick="startGame('william')">🔨 윌리엄 (40세, 숙련 직조공)<br><small style="color: #bbb; font-weight: normal;">기계 도입으로 일자리를 잃어가는 장인</small></button>
    <button class="btn" onclick="startGame('james')">🎩 제임스 (45세, 방적 공장주)<br><small style="color: #bbb; font-weight: normal;">이윤과 생존 경쟁에 직면한 신흥 자본가</small></button>
    <button class="btn" onclick="startGame('mary')">🏠 메리 (24세, 도시 빈민 여성)<br><small style="color: #bbb; font-weight: normal;">비위생적인 지하실에서 가족을 부양하는 노동자</small></button>
  </div>

  <!-- 2. 게임 플레이 화면 -->
  <div id="screen-game" class="hidden">
    <div class="stats-bar">
      <div class="stat-item"><span id="stat-name-1">생존도</span><br><span class="stat-value" id="stat-val-1">100</span></div>
      <div class="stat-item"><span id="stat-name-2">자산/소득</span><br><span class="stat-value" id="stat-val-2">50</span></div>
      <div class="stat-item"><span>현재 라운드</span><br><span class="stat-value" id="round-indicator">1 / 4</span></div>
    </div>

    <div class="card">
      <span class="badge" id="role-badge">역할명</span>
      <h2 id="scenario-title">시나리오 제목</h2>
      <p class="desc" id="scenario-desc">시나리오 본문 내용입니다.</p>
    </div>

    <div id="feedback-area" class="feedback-box hidden"></div>

    <div id="choice-buttons">
      <!-- 선택지 버튼 동적 생성 -->
    </div>
  </div>

  <!-- 3. 엔딩 및 디브리핑 화면 -->
  <div id="screen-ending" class="hidden">
    <h1>시뮬레이션 종료</h1>
    <p class="subtitle">19세기 맨체스터에서의 기록</p>

    <div class="card">
      <h2 id="ending-title" style="color: #e6b422;">엔딩 제목</h2>
      <p class="desc" id="ending-desc">엔딩 해설 본문입니다.</p>
    </div>

    <div class="card" style="background: #1e293b; border-color: #3b82f6;">
      <h2 style="font-size: 1rem; color: #60a5fa;">💡 수업 토론 과제</h2>
      <p class="desc" style="font-size: 0.9rem; color: #cbd5e1; margin-bottom: 0;">
        1. 내가 선택한 인물이 마주했던 가장 가혹한 딜레마는 무엇이었나요?<br><br>
        2. 당시 기계를 부수었던 '러다이트'의 행동과 오늘날 인공지능·키오스크 확산으로 겪는 갈등은 어떤 점이 닮아 있나요?
      </p>
    </div>

    <button class="btn btn-primary" onclick="copyResult()">📋 내 활동 결과 복사하기</button>
    <button class="btn" style="text-align: center;" onclick="location.reload()">🔄 다시 시작하기</button>
  </div>
</div>

<script>
  const scenarios = {
    tom: {
      roleName: "아동 노동자 톰 (11세)",
      stat1: "체력", stat2: "일당(실링)",
      val1: 80, val2: 3,
      rounds: [
        {
          title: "라운드 1: 멈추지 않는 증기 방적기",
          desc: "하루 14시간째 일하고 있습니다. 돌아가는 기계 밑으로 기어들어가 엉킨 실밥을 빼내야 합니다. 졸음이 쏟아집니다.",
          choices: [
            { text: "잠을 쫓기 위해 무리해서 기계 밑으로 들어간다.", f: "기계 톱니에 옷자락이 스쳤지만 간신히 일당을 지켰습니다. (체력 -20)", d1: -20, d2: 0 },
            { text: "잠시 기계 옆 구석에서 눈을 붙인다.", f: "감독관의 가죽 채찍을 맞고 하루 일당이 깎였습니다. (체력 -10, 일당 -1)", d1: -10, d2: -1 }
          ]
        },
        {
          title: "라운드 2: 식수 오염과 도시의 병",
          desc: "공장 폐수와 오물이 섞인 우물물을 마신 동료 아이들이 하나둘 고열로 쓰러집니다.",
          choices: [
            { text: "갈증을 참으며 빗물을 받아 마신다.", f: "탈수를 겪었지만 전염병을 간신히 피했습니다. (체력 -10)", d1: -10, d2: 0 },
            { text: "목이 말라 공장 앞 우물물을 마신다.", f: "배탈과 열병으로 며칠간 앓아누웠습니다. (체력 -30, 일당 -1)", d1: -30, d2: -1 }
          ]
        },
        {
          title: "라운드 3: 공장법 조사관의 비밀 질문",
          desc: "의회에서 파견된 '새들러 위원회' 조사관이 다가와 공장주 몰래 하루 몇 시간 일하는지 묻습니다.",
          choices: [
            { text: "사실대로 하루 15시간 넘게 일한다고 털어놓는다.", f: "조사관은 수첩에 적었지만, 공장주에게 발각될까 두렵습니다.", d1: 0, d2: 0 },
            { text: "해고가 두려워 괜찮다고 거짓말을 한다.", f: "일자리는 지켰지만 열악한 근로조건은 그대로입니다.", d1: -10, d2: 0 }
          ]
        },
        {
          title: "라운드 4: 파업 집회 참여",
          desc: "성인 노동자들이 아동 노동 제한과 임금 보장을 외치며 공장 가동 중단을 요구합니다.",
          choices: [
            { text: "일손을 놓고 형, 누나들의 대열에 합류한다.", f: "공장은 멈췄고 노동의 가치를 깨닫기 시작했습니다.", d1: 0, d2: 0 },
            { text: "보복이 두려워 묵묵히 기계 앞을 지킨다.", f: "하루치 빵은 얻었지만 고립감을 느낍니다. (일당 +1)", d1: -10, d2: 1 }
          ]
        }
      ]
    },
    william: {
      roleName: "숙련 직조공 윌리엄 (40세)",
      stat1: "장인 자부심", stat2: "생활비(실링)",
      val1: 90, val2: 20,
      rounds: [
        {
          title: "라운드 1: 증기 직조기의 습격",
          desc: "평생 수작업으로 최고급 천을 짜왔지만, 공장에서 찍어낸 값싼 직물이 시장을 장악했습니다. 손님이 끊겼습니다.",
          choices: [
            { text: "손기술을 믿고 수공업 방식을 고수한다.", f: "장인의 자존심은 지켰지만 수입이 절반으로 줄었습니다. (소득 -10)", d1: +10, d2: -10 },
            { text: "자존심을 접고 방적 공장의 단순 기계공으로 취직한다.", f: "입에 풀칠은 하게 되었으나 장인의 긍지는 무너졌습니다. (자부심 -30, 소득 +5)", d1: -30, d2: +5 }
          ]
        },
        {
          title: "라운드 2: 네드 러드 장군의 밀서",
          desc: "한밤중에 복면을 쓴 동료들이 찾아왔습니다. '우리의 밥줄을 빼앗은 공장 기계를 부수러 가자'고 제안합니다.",
          choices: [
            { text: "망치를 들고 공장으로 향한다. (러다이트 운동)", f: "증기 직조기 서너 대를 파괴했습니다. 가슴이 뚫리지만 군대의 추적이 두렵습니다. (자부심 +20)", d1: +20, d2: 0 },
            { text: "폭력은 답이 아니라며 의회 탄원서 작성을 권유한다.", f: "동료들로부터 비겁자라는 비난을 들었습니다. (자부심 -20)", d1: -20, d2: 0 }
          ]
        },
        {
          title: "라운드 3: 기계파괴자 사형법 공포",
          desc: "영국 의회가 기계를 파괴한 자를 사형에 처하는 법안을 통과시켰습니다. 군대가 거리에 배치됩니다.",
          choices: [
            { text: "지하 조직으로 숨어들어 끝까지 투쟁한다.", f: "현상수배범이 되어 가족을 떠나 도피 생활을 시작합니다. (소득 -10)", d1: +10, d2: -10 },
            { text: "기계 파괴를 멈추고 노동자 공제 조합을 결성한다.", f: "합법적인 테두리 안에서 서로 돕는 조합을 만듭니다.", d1: +10, d2: 0 }
          ]
        },
        {
          title: "라운드 4: 차티스트 운동과 투표권",
          desc: "노동자에게도 투표권을 달라는 '인민헌장(People's Charter)' 서명 운동이 전국으로 번집니다.",
          choices: [
            { text: "서명 운동의 책임자로 나서며 정치 개혁을 요구한다.", f: "법과 제도를 바꾸는 것이 근본적인 해결책임을 확신합니다.", d1: +20, d2: 0 },
            { text: "당장 먹고살기 바빠 서명을 거부한다.", f: "변화의 기회를 외면한 채 하루하루 연명합니다.", d1: -20, d2: 0 }
          ]
        }
      ]
    },
    james: {
      roleName: "방적 공장주 제임스 (45세)",
      stat1: "공장 자본(£)", stat2: "사회적 평판",
      val1: 500, val2: 50,
      rounds: [
        {
          title: "라운드 1: 최신식 증기기관 도입",
          desc: "경쟁 공장들이 기계를 늘려 단가를 낮추고 있습니다. 우리 공장도 설비를 증설해야 생존할 수 있습니다.",
          choices: [
            { text: "대출을 받아 최신 증기 방적기를 대량 도입한다.", f: "생산량이 3배 뛰었지만 노동자들의 불만이 극에 달합니다. (자본 +200, 평판 -15)", d1: +200, d2: -15 },
            { text: "기존 숙련공들의 일자리를 위해 도입을 미룬다.", f: "노동자들은 환호했으나 제품 가격 경쟁에서 밀립니다. (자본 -100, 평판 +20)", d1: -100, d2: +20 }
          ]
        },
        {
          title: "라운드 2: 야간 작업과 안전장치",
          desc: "주문량이 폭주합니다. 밤샘 작업을 돌려야 납기를 맞출 수 있으나 기계 덮개 안전장치는 아직 없습니다.",
          choices: [
            { text: "안전장치 비용을 아끼고 24시간 철야 가동을 지시한다.", f: "막대한 이윤을 남겼으나 어린 직공 한 명이 손을 다쳤습니다. (자본 +150, 평판 -25)", d1: +150, d2: -25 },
            { text: "비용을 들여 안전 덮개를 설치하고 교대 근무를 도입한다.", f: "단기 수익은 줄었으나 사고가 크게 줄었습니다. (자본 -80, 평판 +25)", d1: -80, d2: +25 }
          ]
        },
        {
          title: "라운드 3: 러다이트의 공습 위협",
          desc: "밤마다 성난 직조공들이 공장 습격을 모의한다는 첩보가 들어왔습니다.",
          choices: [
            { text: "무장 민병대를 고용해 발포 권한을 부여한다.", f: "기계는 지켰으나 유혈 사태로 잔혹한 악덕 자본가로 낙인찍힙니다. (평판 -30)", d1: -50, d2: -30 },
            { text: "노동자 대표를 만나 타협안을 제시한다.", f: "약간의 임금 인상으로 공장 파괴를 막아냈습니다. (자본 -50, 평판 +10)", d1: -50, d2: +10 }
          ]
        },
        {
          title: "라운드 4: 공장법 제정 논란",
          desc: "의회에서 9세 미만 아동 노동 금지 및 노동시간 단축을 규정한 '공장법' 제정이 논의 중입니다.",
          choices: [
            { text: "자유방임주의를 주장하며 법안 반대 로비 자금을 댄다.", f: "규제를 막아 단기 이윤을 지켰으나 역사적 오명을 남깁니다. (자본 +50, 평판 -20)", d1: +50, d2: -20 },
            { text: "로버트 오언처럼 모범 공장 모델을 도입해 노동 환경을 개선한다.", f: "초기 비용은 들었으나 노동자 생산성이 장기적으로 올랐습니다. (자본 -50, 평판 +40)", d1: -50, d2: +40 }
          ]
        }
      ]
    },
    mary: {
      roleName: "도시 빈민 여성 메리 (24세)",
      stat1: "가족 건강", stat2: "주거 안정",
      val1: 70, val2: 40,
      rounds: [
        {
          title: "라운드 1: 축축한 지하 단칸방",
          desc: "햇빛조차 들지 않는 지하 셋방에서 결핵을 앓는 아이와 함께 살고 있습니다. 집세 독촉이 심합니다.",
          choices: [
            { text: "방직 공장에 취직해 매일 14시간씩 일한다.", f: "집세는 냈지만 아이를 돌볼 시간이 전혀 없습니다. (건강 -15, 주거 +20)", d1: -15, d2: +20 },
            { text: "집에서 성냥갑 붙이기 부업을 하며 아이를 돌본다.", f: "아이는 지켰으나 집세를 내지 못해 쫓겨날 위기입니다. (주거 -20)", d1: 0, d2: -20 }
          ]
        },
        {
          title: "라운드 2: 맨체스터 콜레라 대유행",
          desc: "하수구가 없어 골목에 오물이 넘쳐납니다. 옆집 가족이 콜레라로 사망했습니다.",
          choices: [
            { text: "모아둔 비상금을 털어 깨끗한 식수를 사 온다.", f: "식비 부담이 극심하지만 감염은 피했습니다. (주거 -10, 건강 +10)", d1: +10, d2: -10 },
            { text: "어쩔 수 없이 강가의 오염된 공용 우물물을 긷는다.", f: "아이가 고열에 시달리기 시작합니다. (건강 -30)", d1: -30, d2: 0 }
          ]
        },
        {
          title: "라운드 3: 무료 급식소와 구빈원",
          desc: "극심한 불황으로 공장이 문을 닫았습니다. 구빈원에 들어가면 가족이 강제로 격리 수용됩니다.",
          choices: [
            { text: "가족 해체를 피하기 위해 구빈원 대신 길거리 구걸을 택한다.", f: "비참하지만 가족 곁을 지켰습니다. (건강 -10)", d1: -10, d2: 0 },
            { text: "생존을 위해 악명 높은 구빈원으로 들어간다.", f: "굶주림은 면했으나 강제 노역과 가족 격리의 고통을 겪습니다. (건강 +10, 주거 -20)", d1: +10, d2: -20 }
          ]
        },
        {
          title: "라운드 4: 노동자 연대와 사회주의 집회",
          desc: "프리드리히 엥겔스가 쓴 '영국 노동자 계급의 상태' 팸플릿을 든 이들이 집회를 열고 있습니다.",
          choices: [
            { text: "여성 노동자 연대에 가입해 목소리를 낸다.", f: "개인의 불행이 사회 구조의 문제였음을 깨닫습니다.", d1: +10, d2: 0 },
            { text: "두려움에 집회를 피해 집으로 돌아온다.", f: "여전히 어두운 지하방이지만 희망의 실마리를 엿보았습니다.", d1: 0, d2: 0 }
          ]
        }
      ]
    }
  };

  let currentRole = null;
  let currentRound = 0;
  let s1 = 0, s2 = 0;
  let choiceHistory = [];

  function startGame(roleKey) {
    currentRole = scenarios[roleKey];
    currentRound = 0;
    s1 = currentRole.val1;
    s2 = currentRole.val2;
    choiceHistory = [];

    document.getElementById("stat-name-1").innerText = currentRole.stat1;
    document.getElementById("stat-name-2").innerText = currentRole.stat2;
    document.getElementById("role-badge").innerText = currentRole.roleName;

    document.getElementById("screen-intro").classList.add("hidden");
    document.getElementById("screen-game").classList.remove("hidden");

    loadRound();
  }

  function loadRound() {
    updateStatsDisplay();
    document.getElementById("feedback-area").classList.add("hidden");
    
    if (currentRound >= currentRole.rounds.length) {
      showEnding();
      return;
    }

    const data = currentRole.rounds[currentRound];
    document.getElementById("round-indicator").innerText = `${currentRound + 1} / ${currentRole.rounds.length}`;
    document.getElementById("scenario-title").innerText = data.title;
    document.getElementById("scenario-desc").innerText = data.desc;

    const btnContainer = document.getElementById("choice-buttons");
    btnContainer.innerHTML = "";

    data.choices.forEach((c) => {
      const btn = document.createElement("button");
      btn.className = "btn";
      btn.innerText = c.text;
      btn.onclick = () => selectChoice(c);
      btnContainer.appendChild(btn);
    });
  }

  function selectChoice(choice) {
    s1 += choice.d1;
    s2 += choice.d2;
    choiceHistory.push(choice.text);

    const fb = document.getElementById("feedback-area");
    fb.innerText = choice.f;
    fb.classList.remove("hidden");

    const btnContainer = document.getElementById("choice-buttons");
    btnContainer.innerHTML = "";

    const nextBtn = document.createElement("button");
    nextBtn.className = "btn btn-primary";
    nextBtn.innerText = currentRound + 1 < currentRole.rounds.length ? "다음 라운드로 넘어가기 →" : "결과 확인하기 →";
    nextBtn.onclick = () => {
      currentRound++;
      loadRound();
    };
    btnContainer.appendChild(nextBtn);

    updateStatsDisplay();
  }

  function updateStatsDisplay() {
    document.getElementById("stat-val-1").innerText = s1;
    document.getElementById("stat-val-2").innerText = s2;
  }

  function showEnding() {
    document.getElementById("screen-game").classList.add("hidden");
    document.getElementById("screen-ending").classList.remove("hidden");

    const endingTitle = document.getElementById("ending-title");
    const endingDesc = document.getElementById("ending-desc");

    endingTitle.innerText = `${currentRole.roleName}의 여정 종료`;
    endingDesc.innerHTML = `
      당신의 최종 결과:<br>
      • <strong>${currentRole.stat1}:</strong> ${s1}<br>
      • <strong>${currentRole.stat2}:</strong> ${s2}<br><br>
      19세기 전반 맨체스터 노동자들의 평균 수명은 고작 17~20세에 불과했습니다. 개인의 나태함 때문이 아니라 오염된 도시 인프라, 안전장치 없는 기계 설비, 생존권 보장 제도의 부재라는 <strong>구조적 문제</strong> 때문이었습니다.
    `;
  }

  function copyResult() {
    const text = `[1830 맨체스터 활동 기록]\n역할: ${currentRole.roleName}\n최종 상태: ${currentRole.stat1} ${s1} / ${currentRole.stat2} ${s2}\n선택한 주요 경로: ${choiceHistory.join(" -> ")}`;
    navigator.clipboard.writeText(text).then(() => {
      alert("결과가 클립보드에 복사되었습니다! 패들렛이나 과제방에 붙여넣으세요.");
    }).catch(() => {
      alert("복사 권한이 없어 수동으로 화면을 캡처하거나 복사해 주세요.");
    });
  }
</script>

</body>
</html>
