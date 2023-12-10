>## *_"It’s not a bug... It’s an undocumented feature!!!"_*

> [!TIP]
>
> 👋 I'm Alex, a senior software engineer with a fiery passion for full-stack and cloud-native application development. I love creating state-of-the-art, cross-platform applications using cutting-edge technology.
>
> 

---

```typescript
type DevStack = Record<string, string | string[]>;

class SoftwareWizard {
  private devStack2023: DevStack = {
    Toolkit: "Bun",
    Languages: ["TypeScript", "WebAssembly (WASI)", "AssemblyScript (WASM)"],
    "App Frameworks": ["Expo", "Next.js (SSR/SSG/ISR)", "WebXR - Babylon.js"],
    Data: ["AWS DataStore/AppSync", "GraphQL"],
    "Infrastructure (Cloud Native)": "AWS Amplify Gen 1/2",
    "Deploy & hosting": [
      "Amplify Hosting",
      "Cloud Sandbox",
      "Fullstack workflows",
    ],
    Database: ["DynamoDB", "Redshift", "Kinesis"],
    "UI & UX": ["Figma-to-Code", "Amplify Form Builder", "Amplify UI"],
    "Backend Admin (headless CMS)": "Amplify Studio",
    "IDE Stuff": ["VSCode", "Fira Code iScript", "dprint"],
  };

  private formatTools(tools: string | string[]): string {
    return Array.isArray(tools)
      ? tools.map((tool) => `  - ${tool}`).join("\n")
      : `  - ${tools}`;
  }

  getStackList(): string {
    return (
      Object.entries(this.devStack2023)
        .map(
          ([category, tools]) => `\n* ${category}:\n${this.formatTools(tools)}`
        )
        .join("") + "\n\n"
    );
  }

  toString(): string {
    return `👋 I'm Alex, a Senior Full-Stack Software Engineer & Code Alchemist with a 2023 stack: ${this.getStackList()} 🌙 Let's make some digital magic! 🧙‍♂️✨`;
  }
}

const alex = new SoftwareWizard();
console.log(alex.toString());
```



<div align="center">
<img src="https://github.com/fnky/fnky/raw/fnky/img/ie.jpg" alt="Best viewed with Microsoft Internet Explorer" align="center" width="128">
</div>
