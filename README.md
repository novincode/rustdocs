# 🦀 OpenDocs: Modern Rust Documentation

Welcome to **OpenDocs Rust** — a fresh, open-source take on Rust documentation, built by developers, for developers. Tired of the old, dry docs? So was I! My goal is to make learning Rust not just easier, but actually fun and collaborative.

## 🚀 Why This Project?
Rust is an amazing language, but its official docs can feel a bit... 2015. I wanted to create a resource that’s:
- **Modern**: Uses interactive components and beautiful UI (powered by [shadcn/ui](https://ui.shadcn.com/) and custom code blocks)
- **Beginner-friendly**: Clear, concise, and approachable for all backgrounds
- **Collaborative**: Anyone can contribute, improve, and share their knowledge
- **Engaging**: With real-world examples, tips, and a bit of personality

## 🌐 See It Live
Check out the docs at: [learn.codeideal.com/rust](https://learn.codeideal.com/rust)

## ✨ Features
- Interactive, annotated code blocks:

```jsx
<CodeBlock
  language="rust"
  showLineNumbers
  highlightLines={[2, 5, 10]}
  focusLines={[5, 6]}
  wordsToHighlight={["unsafe", "unwrap", "Result"]}
  annotations={[
    { line: 2, message: "This is the main function!", style: "info" },
    { line: 5, message: "Be careful with unsafe code.", style: "warning" },
    { line: 10, message: "Handle errors properly!", style: "error" }
  ]}
>{`
fn main() {
    // Entry point
    let nums = vec![1, 2, 3, 4, 5];
    let sum: i32 = nums.iter().sum();
    unsafe {
        println!("Sum (unsafe!): {}", sum);
    }
    let res: Result<(), &str> = Err("Oops!");
    res.unwrap();
}
`}</CodeBlock>
```

- Use [shadcn/ui](https://ui.shadcn.com/) components for beautiful alerts, tabs, and more
- Supports both GitHub-flavored Markdown and custom components
- Open to contributions from anyone — just fork, branch, and PR!

## 🤝 How to Contribute
1. **Fork** this repo
2. **Create a branch** for your feature or fix
3. **Write or improve docs** using Markdown and our custom components
4. **Open a Pull Request** — let’s make Rust learning awesome together!

## 💡 Philosophy
I’m [novincode](https://github.com/novincode), and I started this project to help the next wave of Rustaceans. Programming should be accessible, modern, and a little bit fun. If you feel the same, join in!

## 📢 License & Credits
OpenDocs Rust is open source and always will be. Inspired by the Rust community, built for everyone.

---

> "Let’s make learning Rust as fearless as writing it."

Happy hacking! 🦀
