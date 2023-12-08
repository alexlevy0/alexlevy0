> _"It’s not a bug... It’s an undocumented feature!!!"_

## Hey there, space cowboy!

> [!TIP]
>
> 👋I'm Alex, a senior full-stack software engineer, with a fiery passion for full-stack and cloud-native app development.
>
> What's important to me? Creating state-of-the-art cross-platform apps that not only scale like a superhero, but also have the budget-friendliness of a superhero costume friperie. Efficiency and effectiveness, without breaking the bank.
>
> In my toolkit? A blend of security and portability that makes my apps ready to leap in a single bound. This lets me mix and match cutting-edge tech n' high-quality software like a tech-savvy chef in a digital kitchen.

---

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

<details>
  <summary>🫨</summary>

```typescript
function LogExecutionTime() {
  return function (
    target: any,
    propertyKey: string,
    descriptor: PropertyDescriptor
  ) {
    const originalMethod = descriptor.value;
    descriptor.value = function (...args: any[]) {
      const start = performance.now();
      const result = originalMethod.apply(this, args);
      const duration = performance.now() - start;
      console.log(`${propertyKey} executed in ${duration}ms`);
      return result;
    };
  };
}

function LogMethod() {
  return function (
    target: any,
    propertyKey: string,
    descriptor: PropertyDescriptor
  ) {
    const originalMethod = descriptor.value;
    descriptor.value = function (...args: any[]) {
      console.log(`Calling method: ${propertyKey}`);
      return originalMethod.apply(this, args);
    };
  };
}

type Constructor<T = {}> = new (...args: any[]) => T;

function WizardSkills<T extends Constructor>(Base: T) {
  return class extends Base {
    castSpell(spell: string) {
      console.log(`Casting spell: ${spell}`);
    }

    readScroll(scroll: string) {
      console.log(`Reading scroll: ${scroll}`);
    }
  };
}

namespace SoftwareWizardry {
  export namespace DevTools {
    export type DevStack = {
      [K in string]: string | string[] | never;
    };

    export class SoftwareWizard extends WizardSkills(Object) {
      private name: string = "Alex";
      private title: string =
        "Senior Full-Stack Software Engineer & Code Alchemist";
      private devStack2023: DevStack = {
        Toolkit: "Bun",
        Languages: [
          "TypeScript",
          "WebAssembly (WASI)",
          "AssemblyScript (WASM)",
        ],
        "App Frameworks": [
          "Expo",
          "Next.js (SSR/SSG/ISR)",
          "WebXR - Babylon.js",
        ],
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

      *formatTools(tools: string | string[] | never): Generator<string> {
        if (Array.isArray(tools)) {
          for (let tool of tools) {
            yield `  - ${tool}`;
          }
        } else {
          yield `  - ${tools}`;
        }
      }

      @LogExecutionTime()
      getStackList(): string {
        return (
          Array.from(
            Object.entries(this.devStack2023),
            ([category, tools]) =>
              `\n* ${category}:\n${Array.from(this.formatTools(tools)).join(
                "\n"
              )}`
          ).join("") + "\n\n"
        );
      }

      @LogMethod()
      toString(): string {
        return `👋 I'm ${this.name}, a ${
          this.title
        } with a 2023 stack: ${this.getStackList()} 🌙 Let's make some digital magic! 🧙‍♂️✨`;
      }
    }
  }
}

const alex = new SoftwareWizardry.DevTools.SoftwareWizard();
console.log(alex.toString());
alex.castSpell("CodeConjuring");
alex.readScroll("AncientAlgorithmScroll");
```

</details>

<div align="center">
<img src="https://github.com/fnky/fnky/raw/fnky/img/ie.jpg" alt="Best viewed with Microsoft Internet Explorer" align="center" width="128">
</div>
