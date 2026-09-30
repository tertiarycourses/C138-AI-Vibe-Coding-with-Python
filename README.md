# AI Vibe Coding with Python

**Build, test and deploy a real Python application with an AI coding assistant, reviewing and owning every line it writes.**

| Course detail | Information |
|---|---|
| Course code | `C138` |
| Programme | Non-WSQ |
| Duration | 2 days · 15 hours (9:30am – 5:30pm, 7.5 instructional hours per day) |
| Hands-on labs | 20, all building one application |
| Registration | [View course details and register](https://www.tertiarycourses.com.sg/ai-vibe-coding-with-python.html) |

## About the course

Official courseware for **AI Vibe Coding with Python** (**C138**), conducted by
**Tertiary Infotech Academy Pte Ltd** (UEN 201200696W).

Learners direct an AI coding assistant to write Python, then review, test and refactor what
it produces. You specify the goal, constraints and expected output; the assistant drafts; you
check the result and own it.

All 20 labs build one connected application, **CardGuard**, a card-transaction fraud
screening system:

```text
Streamlit dashboard  ->  FastAPI service  ->  SQLite
   (analyst UI)          (typed endpoints)    (persistence)
                              ^
                    pandas analytics + rule engine
```

Transaction data is generated locally by [`labs/mockdata.py`](labs/mockdata.py) with a fixed
seed (10,851 transactions, 40 cardholders, 42 seeded fraud cases), so every learner and the
trainer see identical numbers. No real cardholder data is used.

## Learning outcomes

| # | On completion, learners can... |
|---|---|
| **LO1** | Apply vibe coding practices: set up a reproducible Python project with uv, and use an AI coding assistant to scaffold, explain and refactor working code. |
| **LO2** | Design and implement object-oriented Python (classes, encapsulation, inheritance and composition) using AI-assisted conversational design. |
| **LO3** | Build data analytics pipelines with pandas: load, clean, transform, group and aggregate realistic datasets into reportable results. |
| **LO4** | Model and validate data with Pydantic and expose it through a FastAPI application with typed request and response models. |
| **LO5** | Package and deploy a Python application: dependency locking, configuration, containerisation and a running deployed service. |

## Topics covered

| Topic | Coverage | Labs |
|---|---|---|
| **1. Vibe Coding Foundations** | uv projects, AI coding assistants, prompting patterns, AI-assisted refactoring | 1–4 |
| **2. Object-Oriented Programming in Python** | Classes, encapsulation, inheritance, composition, dunder methods | 5–8 |
| **3. Data Analytics with pandas** | DataFrames, cleaning, transformation, GroupBy, aggregation, exception handling | 9–12 |
| **4. Data Modelling with Pydantic and FastAPI** | Typed models, validation, endpoints, request/response schemas, SQLite, pytest | 13–16 |
| **5. Packaging and Deployment** | Streamlit UI, configuration and secrets, uv lockfiles, containers, Docker Compose | 17–20 |

| Day | Schedule |
|---|---|
| **1** | Topic 1 (Labs 1–4), Topic 2 (Labs 5–8), Topic 3 begins (Labs 9–10) |
| **2** | Topic 3 completes (Labs 11–12), Topic 4 (Labs 13–16), Topic 5 (Labs 17–20), then course wrap-up |

## Labs

Each lab folder has a `README.md` with the steps and the code it produces. The combined
notebook [`labs/CardGuard-All-Labs.ipynb`](labs/CardGuard-All-Labs.ipynb) runs every lab in order.

| Lab | Title |
|---|---|
| 1 | [Set Up a Reproducible Python Project with uv](labs/topic1/lab01_set_up_a_reproducible_python_project_with_uv/) |
| 2 | [Write Effective Prompts for an AI Coding Assistant](labs/topic1/lab02_write_effective_prompts_for_an_ai_coding_assista/) |
| 3 | [Review and Correct AI-Generated Code](labs/topic1/lab03_review_and_correct_ai_generated_code/) |
| 4 | [Refactor Working Code Conversationally](labs/topic1/lab04_refactor_working_code_conversationally/) |
| 5 | [Model a Domain with Classes and Dunder Methods](labs/topic2/lab05_model_a_domain_with_classes_and_dunder_methods/) |
| 6 | [Encapsulate State with Properties and Validation](labs/topic2/lab06_encapsulate_state_with_properties_and_validation/) |
| 7 | [Build a Rule Hierarchy with Inheritance and Polymorphism](labs/topic2/lab07_build_a_rule_hierarchy_with_inheritance_and_poly/) |
| 8 | [Compose Rules into an Engine](labs/topic2/lab08_compose_rules_into_an_engine/) |
| 9 | [Load and Explore Transactions with pandas](labs/topic3/lab09_load_and_explore_transactions_with_pandas/) |
| 10 | [Handle Errors with Exceptions](labs/topic3/lab10_handle_errors_with_exceptions/) |
| 11 | [Build Per-Cardholder Baselines with GroupBy](labs/topic3/lab11_build_per_cardholder_baselines_with_groupby/) |
| 12 | [Detect Velocity Bursts with Rolling Time Windows](labs/topic3/lab12_detect_velocity_bursts_with_rolling_time_windows/) |
| 13 | [Replace Hand-Written Validation with Pydantic Models](labs/topic4/lab13_replace_hand_written_validation_with_pydantic_mo/) |
| 14 | [Expose the Screening Engine as a FastAPI Endpoint](labs/topic4/lab14_expose_the_screening_engine_as_a_fastapi_endpoin/) |
| 15 | [Persist Screening Decisions to SQLite](labs/topic4/lab15_persist_screening_decisions_to_sqlite/) |
| 16 | [Test the API with pytest and httpx](labs/topic4/lab16_test_the_api_with_pytest_and_httpx/) |
| 17 | [Build a Fraud Analyst Dashboard with Streamlit](labs/topic5/lab17_build_a_fraud_analyst_dashboard_with_streamlit/) |
| 18 | [Externalise Configuration and Protect Secrets](labs/topic5/lab18_externalise_configuration_and_protect_secrets/) |
| 19 | [Lock Dependencies and Containerise the API](labs/topic5/lab19_lock_dependencies_and_containerise_the_api/) |
| 20 | [Deploy the Full Stack with Docker Compose](labs/topic5/lab20_deploy_the_full_stack_with_docker_compose/) |

Every lab uses [uv](https://docs.astral.sh/uv/). Verified on Python 3.12, pandas 3.0,
Streamlit 1.59 and SQLite 3.47. Labs 19–20 also need Docker.

## Courseware

| Artifact | Files |
|---|---|
| Slide deck | [PPTX](courseware/AI%20Vibe%20Coding%20with%20Python%20%28C138%29-v1.0.pptx) · [PDF](courseware/AI%20Vibe%20Coding%20with%20Python%20%28C138%29-v1.0.pdf) |
| Lesson Plan | [DOCX](courseware/LP-AI%20Vibe%20Coding%20with%20Python%20%28C138%29.docx) · [PDF](courseware/LP-AI%20Vibe%20Coding%20with%20Python%20%28C138%29.pdf) |
| Learner Guide | [DOCX](courseware/LG-AI%20Vibe%20Coding%20with%20Python%20%28C138%29.docx) · [PDF](courseware/LG-AI%20Vibe%20Coding%20with%20Python%20%28C138%29.pdf) · [Markdown](LG-AI%20Vibe%20Coding%20with%20Python%20%28C138%29.md) |
| Labs | [`labs/`](labs/) |

This repository publishes the current courseware version only. Build scripts and superseded
versions are not published.

---

© 2026 Tertiary Infotech Academy Pte Ltd (UEN 201200696W) · [www.tertiarycourses.com.sg](https://www.tertiarycourses.com.sg)
