# web3-toolkits-readme
# ✨ Web3 Toolkits - [mingmingcodes/明码] ✨

# 我的 Web3 工具包 / My Web3 Toolkits

[English](#english-description) | [中文说明](#中文说明)




---

<!-- **Key: Link to the live project website should be prominently displayed!** -->
**🚀 Visit my Toolkits Site:** [https://web3toolkits.mingmingcodes.com](https://web3toolkits.mingmingcodes.com)
<!-- Ensure the link is your actual subdomain -->

---

## 📖 Project Overview

This website is one of my Web3 projects, designed to showcase my front-end programming abilities and my proficiency in using Web3 APIs. The site currently features five toolkit pages: the first four solely retrieve on-chain data without requiring a cryptocurrency wallet connection; the final one can connect to a cryptocurrency wallet, though it only interacts with testnets.

# ! Disclaimer: This website does not collect any private data or information. All functionalities are entirely free to use. Please feel free to test and use it normally!

This website is a collection of practical query tools aimed at Web3 developers and enthusiasts. Throughout this project, I have delved into and practised numerous Web3 front-end development technologies, independently managing the entire process from conceptual design, technology selection, and API integration 금액 최종 배포에 이르기까지. The project currently includes the following core toolkit modules:

*   ENS Resolver
*   Block Information Viewer
*   Network Status Overview
*   Transaction Details Viewer
*   Interactive Personal Token Dashboard

---

## 🌟 Key Features & Highlights

*   **Multi-functional Integration:** A one-stop solution offering a variety of commonly used Web3 query functionalities.
*   **User-Friendly Interface:** Each toolkit module features an intuitive and easy-to-use user interface, with a strong emphasis on responsive design to ensure an excellent experience across different devices.
*   **Real-time Data Retrieval:** Provides real-time on-chain data and market information through integration with leading industry APIs such as Alchemy (or Infura), Etherscan, and CoinGecko.
*   **Front-End Technology in Practice:** Comprehensively developed using the Next.js (React) framework, employing modern front-end technologies like React Hooks, CSS Modules, and asynchronous data handling.
*   **Independent Development & Deployment:** The project was completed independently from scratch and successfully deployed on the Vercel platform.
*   **Continuous Learning & Iteration:** Throughout the development process, I continually learned new concepts and resolved technical challenges encountered.

---

## 🛠️ Tech Stack

*   **Front-End Framework:** Next.js (React)
*   **Programming Language:** JavaScript (ES6+)
*   **Core Libraries:**
    *   `ethers.js` (for interacting with the Ethereum blockchain, handling large numbers, formatting, etc.)
    *   (List other third-party JS libraries if used, e.g., Swiper.js, Particles.js)
*   **Styling Solution:** CSS Modules, (possibly global CSS as well)
*   **Data Sources (APIs):**
    *   Alchemy (or Infura) - For core Ethereum RPC calls (e.g., fetching transactions, block information)
    *   Etherscan API - For auxiliary information such as Gas prices, latest block numbers
    *   CoinGecko API - For fetching cryptocurrency market prices
*   **Deployment Platform:** Vercel
*   **Package Manager:** pnpm
*   **Version Control:** Git & GitHub

---

## 🚀 My Development Journey & Challenges

As a beginner obstáculos前端开发, venturing into the Web3 domain has been an exploration obstáculos充满挑战与机遇. Developing this Web3 Toolkits project has been a significant practical exercise for me to systematically learn and apply Web3-related knowledge.

**Main Difficulties Encountered & Solutions Devised:**

1.  **Understanding Core Web3 Concepts:** Initially, my understanding of concepts such as Gas, transaction hashes, block structures, and ENS resolution was not profound. I progressively built a clear comprehension of these concepts by reading extensive documentation, watching tutorials, and cross-referencing with data returned from actual API calls.
2.  **API Selection & Integration:**
    *   **Challenge:** How to select suitable, free, and stable APIs to obtain the necessary on-chain and market data? How to handle the request limits and data formats of different APIs?
    *   **Solution:** I researched multiple RPC providers (like Alchemy, Infura) and data services (Etherscan, CoinGecko), ultimately choosing the current integrated solution because it struck a good balance in terms of free tier limits, data coverage, and ease of use. During integration, I learned how to construct JSON-RPC requests, handle asynchronous `fetch` operations, and parse and transform data structures returned by various APIs.
3.  **Asynchronous Data Flow & State Management:**
    *   **Challenge:** The pages need to fetch data from multiple APIs simultaneously, with data refreshing efeitos periódicos. How to effectively manage these asynchronous operations, loading states, error states, and the final data display?
    *   **Solution:** I primarily utilised React's `useState` and `useEffect` Hooks. `useEffect` was used to trigger initial data fetching and set up timers, while multiple `useState` Hooks managed different data segments, loading flags, and error messages, ensuring the UI updated correctly according to the data state. For parallel API requests, I learned and used `Promise.allSettled` to improve data retrieval efficiency.
4.  **Front-End UI & Interaction Design:**
    *   **Challenge:** How to design a user interface for each tool that is both practical and aesthetically pleasing? How to implement engaging interactive effects (like background animations, responsive layouts)?
    *   **Solution:** I referred to several excellent Web3 applications and design examples, adopting a minimalist layout and interaction model. During implementation, I experimented with various CSS techniques (such as Flexbox, Grid, CSS Modules, Media Queries) to build responsive interfaces and attempted to integrate some lightweight animation effects.

**What I Achieved in This Project:**

*   Methods for interacting with the blockchain and third-party services via RPC and REST APIs.
*   Mature application of front-end development, state management, and asynchronous programming within a Next.js (React) environment to solve Web3 front-end problems.
*   Increased confidence in independently analysing problems, researching information, and resolving technical difficulties.

---

## 📸 Screenshots/GIF Demo

**1. ENS Resolver**

<img width="749" alt="image" src="https://github.com/user-attachments/assets/ade4fdfe-727e-4d34-a697-ff99240fabf9" />

*(Enter an ENS name (e.g., vitalik.eth) or an Ethereum address (0x...) to query its resolution records.)*


**2. Block Information Viewer**

<img width="731" alt="image" src="https://github.com/user-attachments/assets/ad749a87-c20f-40c9-a382-1773ec6f6c2d" />

*(Enter a block number or "latest" to retrieve detailed block information.)*


**3. Network Status Overview**

<img width="1102" alt="image" src="https://github.com/user-attachments/assets/efb241d7-3f91-4b70-9190-11a6771b1170" />

*(Real-time metrics for the Ethereum mainnet.)*


**4. Transaction Details Viewer**

<img width="797" alt="image" src="https://github.com/user-attachments/assets/3df2f521-6762-404f-967f-67817f29e26e" />

*(Enter an Ethereum transaction hash (TxID) to query detailed information.)*


**5. Interactive Personal Token Dashboard**

<img width="1184" alt="image" src="https://github.com/user-attachments/assets/b093e644-85db-4b2b-9aaf-375a3aa3f42d" />

*(Connect your personal wallet, connect to a testnet, query test token balances, and other functionalities.)*

---

## 🚀 How to Run (Local Development)

The live website is deployed; please visit the link at the top of this document to experience it. The APIs required by the website need to be applied for individually.

If you have been granted access to the codebase and wish to run it locally, please follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [HTTPS or SSH link to your private repository]
    cd [project_directory_name]
    ```
2.  **Install dependencies using pnpm:**
    ```bash
    pnpm install
    ```
3.  **Set up environment variables:**
    *   Copy `.env.local.example` (if provided) to `.env.local`.
    *   Fill in the necessary API Keys in the `.env.local` file (e.g., `NEXT_PUBLIC_ALCHEMY_RPC_URL`, `NEXT_PUBLIC_ETHERSCAN_API_KEY`).
4.  **Run the development server:**
    ```bash
    pnpm dev
    ```
5.  Open your browser and navigate to `http://localhost:3000`.

---

## 🤝 Code Access & Contact

This project represents my learning and exploration成果 in the Web3 front-end domain. The complete source code is currently hosted in a private GitHub repository.

If you are a member of a recruitment team or are interested in the specific technical implementation of the project, my coding style, and practical methods, I would be very pleased to share access to the codebase with you and discuss it further.

**Please contact me via the following:**

*   **Email:** `mingmingcodes@gmail.com`

In your email, please briefly state the name of your recruitment company or team and include your GitHub username. I will respond to you or your institution's recruitment personnel as soon as possible.

Thank you for your understanding and valuable time! I look forward to the opportunity to discuss this project and the broader possibilities of Web3 technology with you in more detail.

---




---

<!-- **关键：项目成品网站链接放在最显眼的位置！** -->
**🚀 访问我的工具站:** [https://web3toolkits.mingmingcodes.com](web3toolkits.mingmingcodes.com)
<!-- 确保链接是你的实际子域名 -->

---

## 📖 项目概述 (Project Overview)
该网站是我的一个Web3项目，旨在展示我的前端编程能力，还有对Web3 API的使用能力，该网站目前有5个工具页，前4个是只调取链上数据的，不用链接加密货币钱包，最后一个可以连接加密货币钱包，不过只调取测试链。

# ！声明本网站不采集任何私人数据或信息，所有功能全部免费，请放心测试，正常使用！

<!--
   
    Web3 Toolkits 是一个面向 Web3 开发者和爱好者的实用工具集合，
    旨在提供便捷的链上信息查询和常用功能。本项目作为我深入学习和实践
    Web3 前端技术的成果，整合了多个独立的、真实场景驱动的工具模块。
-->

这是一个旨在为 Web3 开发者和爱好者提供一系列实用查询工具的集合网站。通过本项目，我深入学习并实践了多项 Web3 前端开发技术，并独立完成了从概念设计、技术选型、API 集成到最终部署的全过程。项目目前包含以下核心工具模块：

*   ENS 解析器
*   区块信息查询器
*   网络状态概览
*   交易详情查询器
*   交互式个人代币仪表盘

---

## 🌟 项目亮点与特色 (Key Features & Highlights)



*   **多功能集成：** 一站式提供多种常用的 Web3 查询功能。
*   **用户友好界面：** 针对每个工具模块设计了直观易用的用户界面，并注重响应式布局，确保在不同设备上的良好体验。
*   **实时数据获取：** 通过集成 Alchemy (或 Infura)、Etherscan、CoinGecko 等行业主流 API，提供实时的链上数据和市场信息。
*   **前端技术实践：** 全面采用 Next.js (React) 框架进行开发，运用了 React Hooks, CSS Modules, 异步数据处理等现代前端技术。
*   **独立开发与部署：** 从零开始独立完成项目，并成功部署到 Vercel 平台。
*   **持续学习与迭代：** 在开发过程中不断学习新知识，解决遇到的技术难题。

---

## 🛠️ 技术栈 (Tech Stack)


*   **前端框架:** Next.js (React)
*   **编程语言:** JavaScript (ES6+)
*   **核心库:**
    *   `ethers.js` (用于与以太坊区块链交互，处理大数、格式化等)
    *   (如果使用了 Swiper.js, Particles.js 等第三方 JS 库，也在此列出)
*   **样式方案:** CSS Modules, (可能还有全局 CSS)
*   **数据来源 (APIs):**
    *   Alchemy (或 Infura) - 用于核心的以太坊 RPC 调用 (如获取交易、区块信息)
    *   Etherscan API - 用于获取 Gas 价格、最新区块号等辅助信息
    *   CoinGecko API - 用于获取加密货币市场价格
*   **部署平台:** Vercel
*   **包管理器:** pnpm
*   **版本控制:** Git & GitHub

---

## 🚀 我的开发之旅与挑战 (My Development Journey & Challenges)



作为一名前端初学者，踏入 Web3 领域对我来说是一次充满挑战和机遇的探索。开发这个 Web3 Toolkits 项目的过程，是我系统学习和应用 Web3 相关知识的重要实践。

**遇到的主要困难与解决思路：**

1.  **理解 Web3 核心概念：** 最初，对于 Gas、交易哈希、区块结构、ENS 解析等概念的理解并不深入。我通过阅读大量文档、观看教程，并结合实际 API 调用返回的数据进行比对和学习，逐步构建起对这些概念的清晰认知。
2.  **API 的选择与集成：**
    *   **挑战：** 如何选择合适的免费且稳定的 API 来获取所需的链上数据和市场数据？如何处理不同 API 的请求限制和数据格式？
    *   **解决：** 我调研了多个 RPC 提供商（如 Alchemy, Infura）和数据服务（Etherscan, CoinGecko），最终选择了目前集成的方案，因为它在免费额度、数据覆盖和易用性上达到了较好的平衡。在集成过程中，我学习了如何构造 JSON-RPC 请求，如何处理异步 `fetch`，以及如何解析和转换不同 API 返回的数据结构。
3.  **异步数据流与状态管理：**
    *   **挑战：** 页面需要同时从多个 API 获取数据，并且数据会定时刷新。如何有效地管理这些异步操作、加载状态、错误状态以及最终的数据展示？
    *   **解决：** 我主要运用了 React 的 `useState` 和 `useEffect` Hooks。通过 `useEffect` 来触发初始数据加载和设置定时器，使用多个 `useState` 来分别管理不同数据片段、加载标志和错误信息，确保 UI 能根据数据状态正确更新。对于并行 API 请求，我学习并使用了 `Promise.allSettled` 来提高数据获取效率。
4.  **前端 UI 与交互设计：**
    *   **挑战：** 如何为每个工具设计既实用又具有一定美感的用户界面？如何实现有趣的交互效果（如背景动画、响应式布局）？
    *   **解决：** 我参考了多个优秀的 Web3 应用和设计案例，采用极简的布局和交互模式。在实现过程中，我尝试了不同的 CSS 技术 (如 Flexbox, Grid, CSS Modules, 媒体查询) 来构建响应式界面，并尝试集成一些轻量级的动画效果。

**从这个项目中我做到了：**

*   通过 RPC 和 REST API 与区块链及第三方服务交互的方法。
*   成熟运用在 Next.js (React) 环境下进行前端开发、状态管理和异步编程的解决Web3前端问题。
*   增强了独立分析问题、查找资料和解决技术难题的信心。

---

## 📸 项目功能截图/GIF演示 (Screenshots/GIF Demo)


**1. ENS 解析器**

<img width="749" alt="image" src="https://github.com/user-attachments/assets/ade4fdfe-727e-4d34-a697-ff99240fabf9" />

*(输入一个 ENS 名称 (如 vitalik.eth) 或以太坊地址 (0x...) 来查询其解析记录。)*


**2. 区块信息查询器**

<img width="731" alt="image" src="https://github.com/user-attachments/assets/ad749a87-c20f-40c9-a382-1773ec6f6c2d" />


*(输入区块号或"latest"获取详细的区块信息。)*


**3. 网络状态概览**

<img width="1102" alt="image" src="https://github.com/user-attachments/assets/efb241d7-3f91-4b70-9190-11a6771b1170" />

*(以太坊主网实时指标)*


**4. 交易详情查询器**

<img width="797" alt="image" src="https://github.com/user-attachments/assets/3df2f521-6762-404f-967f-67817f29e26e" />

*(输入以太坊交易哈希 (TxID) 查询详细信息。)*


**5. 交易详情查询器**

<img width="1184" alt="image" src="https://github.com/user-attachments/assets/b093e644-85db-4b2b-9aaf-375a3aa3f42d" />

*(连接个人钱包，测试网连接，查询测试代币余额等功能。)*
---

## 🚀 如何运行 (本地开发 - 如果你想让别人尝试)

<!--
   “成品网站已部署，请访问上方链接体验。”
    网站所需接口需个人申请：
-->

成品网站已部署，请如果需要查看，请发邮件到 *(mingmingcodes@gmail.com)*。

如果您获得了代码库的访问权限并希望在本地运行，请遵循以下步骤：

1.  **克隆仓库 (Clone the repository):**
    ```bash
    git clone [你私有仓库的HTTPS或SSH链接]
    cd [项目目录名]
    ```
2.  **安装依赖 (Install dependencies using pnpm):**
    ```bash
    pnpm install
    ```
3.  **配置环境变量 (Set up environment variables):**
    *   复制 `.env.local.example` (如果提供了) 为 `.env.local`。
    *   在 `.env.local` 文件中填入必要的 API Keys (例如 `NEXT_PUBLIC_ALCHEMY_RPC_URL`, `NEXT_PUBLIC_ETHERSCAN_API_KEY`)。
4.  **运行开发服务器 (Run the development server):**
    ```bash
    pnpm dev
    ```
5.  打开浏览器访问 `http://localhost:3000`。

---

## 🤝 代码访问与交流 (Code Access & Contact)

本项目代表了我在 Web3 前端领域的学习和探索成果。完整的源代码目前存放于一个私有 GitHub 仓库中。

如果您是招聘团队成员或对项目的具体技术实现、我的编码风格和实践方法感兴趣，我非常乐意与您分享代码库的访问权限，并进一步交流。

**请通过以下方式联系我：**

*   **邮箱:** `mingmingcodes@gmail.com` 
*   

在邮件中，请简要署名您的招聘公司或团队，并附上您的 GitHub 用户名，我将尽快为回复您或您的机构招聘人员。

感谢您的理解与宝贵时间！我期待有机会与您深入探讨这个项目以及 Web3 技术的更多可能性。

---


