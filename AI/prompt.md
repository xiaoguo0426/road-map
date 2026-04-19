### Claude Code 最佳实践

https://code.claude.com/docs/zh-C[Claude-Code.md](assets/Claude-Code.md)
N/best-practices


### 高质量的prompt核心要点：

- 具体
- 丰富
- 少歧义

#### Prompt 的典型构成

- 角色：给AI定义一个最匹配人物的角色，比如[你是一位软件工程师]，[你是一位小学老师]
- 指示：对任务进行描述（越详细越具体）
- 上下文：给出与任务相关的其他背景信息（尤其在多轮交互中）
- 例子：必要时给出举例，学术中成为one-shot learning, few-shot learning或in-context learning; 实践证明其对输出正确性有很大帮助
- 输入：任务的输入信息；在提示词中明确的标识出输入
- 输出：输出的格式描述，以便后继模块自动解析模型的输出结果，比如XML等。