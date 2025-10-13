<p align="center">
  <picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/BizLenz/.github/refs/heads/main/assets/logo/logo_dark.svg">
  <img src="https://raw.githubusercontent.com/BizLenz/.github/refs/heads/main/assets/logo/logo_light.svg" width="130" alt="Logo for BizLenz">
</picture>
</p>

<h1 align="center">
  BizLenz
</h1>

<p align="center">
  AI-powered business proposal analysis tool for the web
</p>

> BizLenz는 과학기술정보통신부 대학디지털교육역량강화사업의 지원을 통해 수행한 한이음 드림업 프로젝트 결과물입니다.
>
> BizLenz is the outcome of the Hanium Dream-Up Project, carried out with support from the Ministry of Science, Korea and ICT’s University Digital Education Capacity Enhancement Program.

## BizLenz

This project is a platform that utilizes AI to identify areas for improvement in business plans.

- **NLP-based Business Plan Evaluation Model:** Establishes a methodology for evaluating business plans and designs an AI evaluation model capable of performing both quantitative and qualitative analyses.
- **AI-based Business Plan Diagnostic System:** Builds an AI system that analyzes the content of business plans and assesses their logical flow and validity.

and planned other features, i.e.:

- **Automated Business Model Canvas Generation System:** Automatically generates a BMC based on the content of the business plan.
- **API Provision:** Provides the systems in API form, enabling integration with external services.
- **Team-based Functionalities:** Invite team members in a specific workspace.

### The Problem

Entrepreneurs write business plans for various reasons—such as applying for government support programs, competitions, or attracting investment—but they often struggle to create them effectively.

> “Universities with smaller scales and poor financial conditions cannot even consider consulting. The cost of consulting easily exceeds 100 million KRW per month, depending on the number of consultants dispatched and the time spent.”
>
> _According to [한국대학신문, 2015](#ref-hanguk2015)_

Although mentoring and consulting services from startup mentors, accelerators, and venture capital reviewers exist to address this issue, **only a small number of entrepreneurs can afford to use these solutions** due to many constraints, majorly cost and time.

### Goal

| Category                                            | Limitations of Existing Approach                                                         | Differentiating Features                                                                                                                                                                |
| --------------------------------------------------- | ---------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Business Plan Evaluation**                        | Inconsistency in results due to subjective evaluation by experts                         | **NLP-based AI Analysis:** Uses natural language processing to assess logical consistency and business model relevance, providing consistent evaluation                                 |
| **Quantitative / Qualitative Analysis Integration** | Reliance on evaluators’ experience for qualitative judgment; lack of objective standards | **AI Scoring Algorithm:** Quantifies key business elements through keyword/context analysis; establishes indicators using TF-IDF and BERT-based document embeddings                     |
| **Real-time Feedback**                              | Requires waiting for consulting feedback; difficult to receive iterative feedback        | **Adaptive Feedback System:** Reflects feedback in real time and provides optimal guidance                                                                                              |
| **Customized Analysis**                             | Provides only simple diagnostic results; unclear improvement direction                   | **Automatic BMC Generation and Visualization:** AI analyzes the business plan and automatically generates a Business Model Canvas; delivers intuitive graphical dashboard visualization |
| **Document Optimization & Auto-Improvement**        | Manual, repetitive process needed to apply feedback                                      | **AI-powered Document Enhancement:** Uses GPT-based rewriting and summarization to automatically optimize documents                                                                     |
| **Data Learning & Application**                     | Learning limited by evaluator’s experience and competence                                | **User Feedback Learning AI:** Continuously improves AI model using user feedback; evolves into tailored analysis models for different entrepreneur types                               |

#### Key Differentiation Points

- Provides **objective, highly reliable business plan evaluation**
- Enables **consistent evaluation standards** through AI-based, data-driven analysis rather than subjective interpretation
- Offers **quantitative evaluation indicators** using NLP-based text analysis to enhance evaluation reliability
- Supports **fast document improvement feedback**, allowing entrepreneurs to refine content immediately without delays
- Enhances **business plan completeness** through iterative AI feedback cycles
- Automatically identifies and visualizes **core business elements** as a Business Model Canvas for strategic business understanding
- Delivers **significant time and cost savings** by enabling self-driven evaluation and revision anytime
- Creates **new market opportunities** through technical differentiation, domain-specific NLP models, and AI evaluation systems
- Potential for **patentable innovation** in AI-based automated evaluation and feedback generation technology

### Main Features

- Business evaluation and result export tailored to specific programs (e.g., [예비창업패키지(Pre-startup package, Korea)](https://www.kised.or.kr/menu.es?mid=a10205010000))
- Web application, based on dashboard-first UI  
- Result tracking and management

#### Planned Features

- Visualization (Business Model Canvas generator)
- API integration for external service connectivity
- Team-based features

## Development

Codes were managed in GitHub, using GitHub Flow. Files that are not codes were managed and shared using Google Drive and Notion, and meetups were held on Discord and Zoom.

### System Architecture

#### Frontend Architecture

<img src="https://raw.githubusercontent.com/BizLenz/.github/refs/heads/main/assets/architecture/www_architecture.svg" alt="www_architecture" width="600"/>

#### Backend Architecture

<img src="https://raw.githubusercontent.com/BizLenz/.github/refs/heads/main/assets/architecture/api_architecture.svg" alt="api_architecture" width="400"/>

## Frontend

The frontend was developed using the Next.js framework as it enables server‑side rendering, optimized performance, and efficient integration of dynamic AI‑driven content.

It heavily utilizes the [shadcn/ui](https://ui.shadcn.com/) component library, allowing rapid interface development and maintaining consistent design efficiency even with a single developer on the FE side.

The source code is avaliable at [BizLenz Frontend](https://github.com/BizLenz/www).

## Backend

The backend was developed using the FastAPI framework to ensure seamless integration with AI systems.

The source code is avaliable at [BizLenz Backend](https://github.com/BizLenz/api).

## AI

Using the Gemini 2.5 Flash and Gemini 2.5 Pro models, we enabled automated evaluation through prompt engineering.

The primary focus was on **consistency**, ensuring that when the same file was provided as input, variations in output scores were minimized.

To achieve this, the evaluation process was divided into sections corresponding to actual evaluation criteria, providing clear and explicit standards for each part.

This approach enabled the model to perform consistent assessments. The evaluation results for each section were generated and then comprehensively reviewed before being exported in JSON format.

## Expected Outcomes

- **Establishment of an Objective and Reliable Business Plan Evaluation System**

  - Replaces traditional subjective and experience-based evaluations by experts with an AI-driven approach, delivering consistent results based on unified standards.
  - Enhances evaluation reliability through NLP-based sentence and context analysis that objectively assesses logic, marketability, and business model suitability.

- **Improvement of Document Quality through Real-time Feedback**

  - AI instantly provides feedback and improvement directions, enabling entrepreneurs to refine business plans without waiting for consulting sessions.
  - Iterative feedback allows continuous refinement, enhancing document completeness and competitiveness.

- **Automated Business Model Analysis and Visualization**

  - AI automatically extracts key elements from business plans, converts them into a Business Model Canvas (BMC), and provides visual outputs for strategic insights.
  - Enables investors and evaluators to intuitively understand the business structure, improving persuasive communication.

- **Time and Cost Reduction**

  - Reduces dependence on expert consulting, allowing entrepreneurs to access AI-based evaluation and feedback at low cost anytime.
  - Significantly shortens business plan preparation time for early-stage startups and small teams, improving overall operational efficiency.

- **Creation of New Market Opportunities through Technological Differentiation**

  - Builds a foundation for global expansion and new revenue models through patents and IP strategies based on AI-driven automated evaluation and feedback technology.

## Application Areas

- **Investment Attraction**

  - Strengthens investor persuasion by presenting clear quantitative indicators of business strengths and weaknesses through AI-driven data analysis.
  - Incorporates investment evaluation criteria into the AI, allowing entrepreneurs to anticipate potential additional data requests and risk factors during due diligence.

- **Startup Promotion**

  - Enables first-time entrepreneurs to efficiently and systematically draft business plans using AI’s step-by-step guidance and feedback.
  - Provides automated evaluation and improvement guides for government support programs and startup competitions, reducing preparation time and improving quality.
  - Iterative feedback and learning functions help founders refine their strategies and improve documentation autonomously.
  - Creates an environment where entrepreneurs can validate and evolve business ideas independently, lowering barriers to entry.

- **Corporate Project Activation**

  - Supports fast and rational decision-making for new business reviews by quantitatively and qualitatively analyzing market trends, business models, and risks.
  - Provides data-driven insights for feasibility, profitability, and marketability assessments applicable to internal ventures, product development, and market expansion.
  - Enhances the success rate of in-house venture programs and minimizes risk in new business initiatives.

- **Education Sector**

  - Serves as a practical tool for business plan writing and evaluation training in universities, corporations, and entrepreneurship education institutions.
  - Provides learners with real-case-based analysis and feedback experience to develop applied understanding and competency.
  - Enables educational institutions to use system-generated data to design data-driven curricula and manage project-based learning more effectively.

- **Consulting Industry Collaboration and Market Expansion**
  - Consulting firms can enhance reliability and efficiency by integrating AI analytics for standardized and objective insights.
  - Consultants can leverage AI-generated qualitative and quantitative data to improve consistency, reduce effort, and optimize consulting quality and cost.

## Team

- [7591yj](https://github.com/7591yj)

  - Team leader, project management
  - FE designs with Figma
  - Frontend development with Next.js
  - Contributed on the API/ERD specification
  - Prompt engineering
  - Depolyment process on AWS (FE)

- [최정인](https://github.com/chlwjddls0923)

  - BE development with FastAPI
  - DB management with PostgreSQL
  - Deployment process on AWS

- [Soborobang1](https://github.com/Soborobang1)

  - BE development with FastAPI
  - CI management with GitHub Actions
  - Wrote test codes for the backend

---

### Citations

- <a name="ref-hanguk2015"></a>한국대학신문. (2015). _프라임 사업에 사설 컨설팅 업체 ‘활개.’._ <http://news.unn.net/news/articleView.html?idxno=152928>.
