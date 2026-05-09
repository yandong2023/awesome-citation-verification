# AI 写作时代，为什么一定要做参考文献真实性检查

如果你用 ChatGPT、Claude 或其它 AI 工具辅助写过论文、综述、开题报告、基金申请、医学写作稿，大概率会遇到一个很尴尬的问题：

文字看起来很像那么回事，参考文献也排得整整齐齐，但这些文献到底是不是真的？

更麻烦的是，有些引用不是“一眼假”。它们可能长这样：

- DOI 是真的，但对应的是另一篇文章。
- 作者和年份看起来对，标题却对不上。
- 论文真实存在，但根本不支持你这句话。
- AI 把几篇文章的信息拼在一起，生成了一条“看起来很真实”的假参考文献。
- 综述里提到过这个观点，但真正的一手证据其实在另一篇原始研究里。

这就是为什么我们需要做 citation verification，也就是参考文献真实性和可辩护性检查。

## 参考文献不是“能搜到”就够了

很多人检查参考文献，只做了一步：把标题或 DOI 放到 Google Scholar、PubMed、Crossref 里搜一下。

这当然有用，但远远不够。

一条引用真正合格，至少要回答几个问题：

1. 这篇文章是否真实存在？
2. DOI、标题、作者、年份、期刊是否匹配？
3. 它是不是被 PubMed、Crossref、OpenAlex 或出版社页面收录？
4. 它是否真的支持正文里的那句话？
5. 如果导师、审稿人、客户追问，我能不能解释为什么引用它？

前 3 个问题是“引用是否真实”。第 4 和第 5 个问题，才是“引用是否站得住”。

## AI 假文献最危险的地方：它不像错的

以前参考文献出错，往往是格式问题：页码错了、期刊缩写错了、年份漏了。

现在的问题更隐蔽。

AI 生成的假引用经常有完整的作者、标题、期刊、年份、卷期页码，甚至还有一个看起来合理的 DOI。对没有时间逐条核查的人来说，它非常容易混进 bibliography。

而一旦进入投稿、毕业论文、医学写作交付、客户报告，风险就不是“格式扣分”这么简单了。

它会直接影响可信度：

- 导师会怀疑整篇文章是否认真。
- 审稿人会质疑作者是否核对过来源。
- 医学写作客户会担心合规和专业风险。
- AI 辅助写作的价值会被一条假引用拖累。

所以参考文献检查不应该放在最后一分钟，而应该变成写作流程里的一道固定安全检查。

## 一个实用的参考文献检查流程

你可以按这个顺序做：

1. 从文稿中提取所有 references。
2. 逐条检查 DOI、PMID、PMCID 或 URL 是否存在。
3. 对比标题、作者、年份、期刊、卷期、页码。
4. 在 PubMed、Crossref、OpenAlex、Semantic Scholar 或出版社页面确认记录。
5. 回到正文，看这条引用对应的是哪一句话。
6. 阅读摘要、结果、图表或全文，判断它是否真的支持这个 claim。
7. 给每条引用标记状态：已验证、需复核、不匹配、未找到、不支持正文表述。
8. 在提交前替换掉高风险引用。

这个流程听起来有点慢，但它能避免很多后面更麻烦的返工。

## 建议使用的状态标签

检查 bibliography 的时候，不要只写“对”或“不对”。建议用更细的标签：

| 状态 | 含义 |
| --- | --- |
| `verified` | 元数据匹配，并且来源基本支持正文表述。 |
| `metadata mismatch` | 文献存在，但 DOI、标题、作者、年份或期刊信息不匹配。 |
| `not found` | 没有在可靠数据库或出版社页面找到这条记录。 |
| `suspicious` | 具有明显 AI 编造、拼接或复制错误的迹象。 |
| `does not support claim` | 文章真实存在，但不支持正文里的那句话。 |
| `needs manual review` | 自动检查或初步检查无法判断，需要人工进一步确认。 |

这样做的好处是：你最后拿到的不是一个模糊的“查过了”，而是一份可以交付、可以复盘、可以解释的 citation integrity report。

## 什么时候最需要做这件事？

特别建议下面几类场景做引用检查：

- 用 AI 辅助写过文献综述。
- 论文里有一批参考文献是临时补上的。
- 返修时需要回应 reviewer 对证据的要求。
- 医学写作稿件需要交付给客户或机构。
- 参考文献来自 ChatGPT、Claude、Perplexity 或其它 AI 工具。
- 文章准备投稿、毕业提交或正式发布。

不是所有文献都需要做很重的人工核查，但所有“看起来重要的引用”都应该能经得起追问。

## 用 LitSource 更快完成这件事

如果你只想手动查，可以使用本仓库里的清单和模板：

- [检查一条参考文献是否真实](checklists/check-if-a-reference-is-real.md)
- [Citation Integrity Report 模板](templates/citation-integrity-report.md)
- [可疑参考文献模式](examples/suspicious-reference-patterns.md)

如果你想更快一点，可以用 LitSource：

- 参考文献检查：https://litsource.net/zh/citation-checker?utm_source=github&utm_medium=repo&utm_campaign=awesome-citation-verification-zh
- 反查文献：https://litsource.net/zh/reverse-literature-search?utm_source=github&utm_medium=repo&utm_campaign=awesome-citation-verification-zh
- ChatGPT 假参考文献检查：https://litsource.net/zh/chatgpt-fake-references-checker?utm_source=github&utm_medium=repo&utm_campaign=awesome-citation-verification-zh

LitSource 的目标不是替你“盲目相信 AI”，而是帮你把引用检查变得更可追溯、更可审计、更可辩护。

## 最后一句话

AI 可以帮你更快写作，但不能替你承担引用错误的责任。

真正专业的写作，不只是把参考文献放在文末，而是确保每一条关键引用都真实、匹配、支持正文，并且经得起导师、审稿人和客户追问。

