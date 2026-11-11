边界用例（用于校验输入规则，不进入完整流程）

一、缺难度标签：把 case-1-cet4.md 的正文发出，但不带「难度标签：四级」这一行。
预期：只追问难度标签，不输出任何概况、问题或讲解。

二、文本过短：以下正文 62 词左右。
预期：先提示"文本偏短"，等用户确认再继续。

Most people believe that a good night's sleep depends on the length of time they spend in bed. Researchers now disagree. What matters, they argue, is not how many hours a sleeper collects but how regular the schedule is. A person who goes to bed at the same time every night, even for only six hours, often feels fresher than someone who sleeps eight hours at unpredictable times.
