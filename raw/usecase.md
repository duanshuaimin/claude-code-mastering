# In-depth Analysis of Claude Code Usage by Anthropic Teams

*This article is reconstructed based on the internal report "How Anthropic teams use Claude Code" (2025) published by Anthropic.*

---

## Introduction

Anthropic is integrating **Claude Code** into its operations across all departments, expanding productivity not only for developers but also for non-developers. Below, we detail how each organization utilizes Claude Code, for what purposes and in what ways, and the resulting effects and practical tips.

---

## 1. Data Infrastructure Team

### Team Role

* Building and operating enterprise-wide data pipelines

### Key Usage Scenarios

* **Kubernetes Failure Diagnosis**: Inputting screenshots to identify dashboard warnings and even receive guidance on IP pool expansion commands.
* **Plain-text Workflow Execution**: Non-developers describe procedures in text format, and Claude Code automatically generates queries and reports.
* **New Staff Onboarding**: Reading `Claude.md` documents to explain codebase and pipeline dependencies.
* **Documentation at Session End**: Automatically recording work summaries and improvement suggestions to continuously enhance document quality.
* **Multi-instance Parallel Work**: Maintaining separate sessions per repository to switch contexts without loss.

### Team Achievements

* Cluster recovery without network expert intervention.
* Accelerated contribution speed of new data analysts.
* Automated monitoring of over 200 dashboards for anomaly detection.

### Practical Tips

* Write detailed workflow and tool descriptions in `Claude.md` documents.
* For sensitive data processing, **MCP server** is recommended instead of BigQuery CLI.
* Propagate best practices by sharing usage sessions within the team.

---

## 2. Product Development Team

### Team Role

* Expanding Claude Code's own features and developing core logic.

### Key Usage Scenarios

* **Autonomous Iterative Prototyping (shift+tab mode)**.
* **Synchronous Pair Coding** for quality management of core business logic implementation.
* Over 70% automated implementation of peripheral features like **Vim mode**.
* **Test and bug fix automation** and GitHub Actions integration.
* Reduced learning time through **large-scale monorepo navigation**.

### Team Achievements

* Reduced implementation time for complex features and improved quality.
* Expanded test coverage, secured release stability.

### Practical Tips

* Include build, test, and lint verification in autonomous loops.
* Differentiate between asynchronous vs. synchronous methods based on task importance.
* Specify prompts more concretely when there are many similar names.

---

## 3. Security Engineering Team

### Team Role

* SDLC security, strengthening supply chain and development environment security.

### Key Usage Scenarios

* **Stack trace tracking** reduced incident resolution time from 10 to 5 minutes.
* **Terraform change review automation** resolved approval bottlenecks.
* **Document integration and runbook generation** for real-time reference.
* Established **Test-Driven Development (TDD)** patterns.

### Team Achievements

* Accelerated incident response.
* Shortened infrastructure security review cycles.

### Practical Tips

* Actively use custom slash commands (accounts for 50% of monorepo commands).
* Employ a “Let Claude talk first” strategy to encourage autonomous resolution.
* Actively apply it to document writing and formatting tasks.

---

## 4. Inference Team

### Team Role

* Managing and improving model memory systems.

### Key Usage Scenarios

* Instant support for **codebase structure understanding**.
* **Automated unit test generation** and reinforcement of missing edge cases.
* Eased learning curve with **ML concept explanations**.
* Secured tests through **multilingual code conversion** (e.g., Rust).
* **Kubernetes command reference** always available.

### Team Achievements

* Reduced ML research learning time by 80%.
* Streamlined code navigation and test writing.

### Practical Tips

* Judge utility by comparing knowledge-based answer speed with Google Search.
* Build trust through code generation → verification stages.
* Habituate automated test generation.

---

## 5. Data Science & Visualization Team

### Team Role

* Developing visualizations and dashboards for model performance analysis.

### Key Usage Scenarios

* Fully automated creation of a **React/TypeScript** based dashboard of 5,000 lines.
* Automated **iterative refactoring** tasks in a ‘slot machine’ manner.
* Transition from **one-off notebooks to permanent dashboards**.
* Achieved productivity even with unfamiliar tech stacks through **zero-dependency task delegation**.

### Team Achievements

* 2-4x reduction in task time.
* Ability to implement complex apps even in non-specialized languages.

### Practical Tips

* An effective strategy is to roll back to an initial state upon failure and retry.
* Periodically request simplification instead of complex solutions.

---

## 6. API Knowledge Team

### Team Role

* Developing and testing knowledge expansion features like PDF, citation, and web search.

### Key Usage Scenarios

* Reduced initial context gathering time by **identifying files before tasks**.
* Improved self-reliance in **debugging other codebases**.
* Direct feedback through **dogfooding research model snapshots**.
* **Reduced context switching**: No need to copy/explain code.

### Team Achievements

* Increased confidence in solving problems in unfamiliar areas.
* Reduced onboarding time and improved developer satisfaction.

### Practical Tips

* Approach with a repetitive collaboration perspective rather than expecting one-off answers.
* Expand based on Claude's guidance after providing minimal information.

---

## 7. Growth Marketing Team

### Team Role

* Building and operating performance marketing channels (search, social, app, etc.).

### Key Usage Scenarios

* **Automated Google Ads creative generation**: CSV analysis → generation of variations for low-performing ads.
* Mass production of 100 types of image assets with a **Figma plugin**.
* Campaign analysis automation via **Meta Ads MCP server**.
* Reusing experiment logs with a **memory system**.

### Team Achievements

* Ad copy creation time reduced from 2 hours to 15 minutes, 10x creative production.
* Achieved engineering-level automation despite being a 1-person team.

### Practical Tips

* Select repetitive tasks of API-providing tools as automation targets.
* Divide complex workflows into sub-agents.
* Recommend designing ideas first, then executing them step-by-step.

---

## 8. Product Design Team

### Team Role

* UI/UX design and improvement across Claude Code, Claude.ai, and APIs.

### Key Usage Scenarios

* Designers directly implement **frontend visual and state management modifications**.
* Automated code suggestions for **GitHub Actions** issues alone.
* Instant generation of interactive prototypes based on **image pasting**.
* Proactive edge case identification with **system state and error flow maps**.
* Bulk search and replacement for **large-scale copy changes**.

### Team Achievements

* Designers perform developer-level tasks, improving speed 2-3x.
* Reduced complex message replacement tasks from 1 week to about 1 hour.

### Practical Tips

* Initial setup (repo permissions, etc.) requires engineer assistance.
* Specify designer roles and detailed feedback requests in a `memory` file.
* Actively utilize screenshot-based code generation.

---

## 9. RL Engineering (Reinforcement Learning) Team

### Team Role

* Developing large-scale sampling and weight transfer systems.

### Key Usage Scenarios

* Implemented authentication features, etc., with **supervised autonomous code writing**.
* Automated **testing and reviews**.
* Understood complex code structures with **call stack summaries**.
* Instant queries for **Kubernetes operation guides**.

### Team Achievements

* Established a safe 'try then rollback' experimentation culture.
* Reduced documentation burden with automated comment generation.

### Practical Tips

* Add rules to `Claude.md` to prevent recurring errors.
* Ensure experiment safety by committing checkpoints frequently.
* Attempt full implementation first, then switch to collaboration mode.

---

## 10. Legal Team

### Team Role

* Product and regulatory compliance review, and internal legal support.

### Key Usage Scenarios

* **Personal accessibility tool**: Prototyped a predictive text assistance app in 1 hour.
* Automated responsible attorney matching with **‘phone tree’ simulation**.
* Review status tracking with **G Suite automation**.
* Expert verification with **visual-centric prototyping**.

### Team Achievements

* Demonstrated the possibility for non-developers to implement custom legal tools.
* Focused on high-value tasks by automating repetitive work.
* Promoted idea verification and sharing through prototyping.

### Practical Tips

* Design thoroughly in Claude.ai before implementing with Claude Code.
* Utilize step-by-step execution and screenshot feedback loops.
* Share prototypes for collaboration even if incomplete.

---

## Conclusion

These Anthropic case studies show that **Claude Code**, beyond being a simple code generation tool, can function as a **multi-role agent** that reshapes how organizations solve problems, automate tasks, and collaborate. By optimizing prompt strategies and workflow designs tailored to their specific job characteristics and technical proficiency, each team has simultaneously boosted development speed, quality, and inter-organizational collaboration efficiency.

