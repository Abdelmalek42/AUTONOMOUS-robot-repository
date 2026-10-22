# AUTONOMOUS-robot-repository
new project , welcome
dhia is here
FinRobot/
├── finrobot_autogen/            # V0 — AutoGen generation (PyPI: pip install finrobot)
│   ├── finrobot/                #   package root — imported as `finrobot`
│   │   ├── agents/              #     agent_library.py, workflow.py, prompts.py
│   │   ├── data_source/         #     finnhub / finnlp / fmp / sec / yfinance / reddit
│   │   ├── functional/          #     analyzer, charting, coding, quantitative, rag, text
│   │   ├── toolkits.py          #     registers Python functions as agent tools
│   │   └── utils.py
│   ├── tutorials_beginner/      #   hands-on tutorials
│   ├── tutorials_advanced/      #   advanced tutorials for FinRobot developers
│   ├── experiments/             #   investment group, multi-factor, portfolio optimization
│   ├── configs/ report/         #   agent configs and sample generated reports
│   ├── FinNLP/                  #   git submodule
│   ├── OAI_CONFIG_LIST_sample
│   ├── config_api_keys_sample
│   └── requirements.txt
│
├── finrobot_desktop/            # V2 — PydanticAI desktop generation (current)
│   ├── finrobot/                #   Python backend (FastAPI + compute engine)
│   │   ├── engine/              #     agents/, pipelines/, compute/, data/
│   │   ├── artifact/            #     report store + output contract gate
│   │   ├── audit/ coverage/ obs/ routes/
│   │   └── cli.py server.py sdk.py
│   ├── desktop/                 #   Tauri shell + React frontend (src/, src-tauri/)
│   ├── skills/                  #   56 analyst playbooks
│   ├── tests/ scripts/ tutorials/
│   └── pyproject.toml uv.lock dev.sh
│
├── finrobot_equity/             # V1 — OpenAI Agents SDK generation
│   ├── core/                    #   analysis engine + 8 section-writing agents
│   ├── web_app/                 #   FastAPI web application
│   ├── run_web_app.py           #   launcher
│   ├── deploy.sh                #   local deployment
│   ├── deploy.gcloud.sh         #   Cloud Run deployment
│   └── requirements.txt
│
├── Dockerfile .dockerignore     # V1 container build — must stay at the repo
│                                # root, since the image imports the app as
│                                # finrobot_equity.web_app.main
├── .github/workflows/           # desktop CI (backend 3.11/3.12, frontend Node 22/24)
├── setup.py                     # packages V0 (as `finrobot`) + V1 for PyPI
├── LICENSE NOTICE TRADEMARK_POLICY.md
└── README.md
