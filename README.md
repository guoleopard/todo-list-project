# Todo List 项目题目

## 任务概述
实现一个包含前端（Vue）和后端（Pythoh+Fastapi）的简易 Todo List Web 应用，功能聚焦在任务的增删改查以及用户的基本认证。项目要求代码结构清晰、前后端分离，并提供 Docker Compose 一键启动脚本。

## 功能要求
1. **用户模块**
   - 注册、登录（基于 JWT）
   - 查看/修改个人信息
2. **任务模块**
   - 新增任务（标题、描述、截止日期）
   - 查看任务列表（支持分页）
   - 标记任务完成/未完成
   - 编辑任务内容
   - 删除任务
   - 按完成状态或截止日期筛选任务
3. **前端要求**
   - 使用 Vue 实现单页应用
   - UI 简洁，建议使用 Ant Design、Material‑UI 等组件库
   - 与后端 RESTful API 完成交互，展示加载、错误提示
4. **后端要求**
   - Python + Fastapi，使用 Mysql 持久化数据
   - 提供符合 REST 规范的 API，实现用户认证、任务 CRUD
   - 对所有入口进行基本的输入校验与错误处理
5. **部署**
   - 编写 `docker-compose.yml`，包含前端、后端、数据库三层服务
   - 提供 `docker-compose up --build` 一键启动命令

## 项目结构（示例）
```
.todo-list-project/
├─ frontend/      # Vue 项目代码
├─ backend/       # Fastapi 项目代码
├─ db/            # 数据库初始化脚本
├─ docker-compose.yml
└─ README.md
```

## 评分要点
- 前后端代码组织合理、符合最佳实践
- API 设计清晰，错误处理到位
- 前端交互流畅，界面友好
- Docker 配置完整，可在本地快速启动
- 代码中包含基本的单元测试（可选）

## 提交要求
- 所有实现均提交到 `dev` 开发分支
- 完成功能后通过 Pull Request 合并到 `main`
- PR 中需写明实现的功能点与已知的限制

---

祝你完成项目顺利！
