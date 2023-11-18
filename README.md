> *"It’s not a bug... It’s an undocumented feature!!!"*

## Hey there, space cowboy!

> [!TIP]
> 
>👋 I'm Alex, a up-and-comer of code and a senior full-stack software engineer, with a fiery passion for full-stack and cloud-native app development, sprinkled with a dash of tech magic and a bit of sparkle.
>
>My forte? Creating state-of-the-art cross-platform apps that scale like a superhero, cost-effective as a buy-one-get-one-free sale, while maintaining security tighter than Fort Knox and portability that could leap over the moon.
>
>This approach allows me to mix and match cutting-edge tech like a DJ, consistently dishing out high-quality software in the twisty, turvy world of software engineering. And there you have it!
>

---
---
```typescript
type DevStack = {
  [key: string]: string | string[];
};

class SoftwareWizard {
  private name = "Alex";
  private title = "Senior Full-Stack Software Engineer & Code Alchemist";
  private devStack2023: DevStack;

  constructor() {
    this.devStack2023 = {
      "Languages": ["TypeScript", "AssemblyScript"],
      "App Frameworks": ["Expo.dev", "Babylon.js"],
      "AWS Amplify": ["GraphQL/AppSync", "Amplify Studio"],
      "Infrastructure & Database": ["DynamoDB", "CloudFormation"],
      "UI & UX": ["Figma-to-Code - Amplify Form Builder", "Amplify UI"]
    };
  }

  getStackList(): string {
    return Object.entries(this.devStack2023)
      .map(([category, tools]) => `${category}: ${Array.isArray(tools) ? tools.join(", ") : tools}`)
      .join("; ");
  }

  toString(): string {
    return `👋 I'm ${this.name}, a ${this.title} with a 2023 stack: ${this.getStackList()}. 🌙 Let's make some digital magic! 🧙‍♂️✨`;
  }
}

const alex = new SoftwareWizard();
console.log(alex.toString());
```

## GitHub Stats

![Metrics](https://metrics.lecoq.io/alexlevy0)

## Contact Info

- Email: [alexlevy0@gmail.com](mailto:alexlevy0@gmail.com)
- LinkedIn: [Alex Lévy](https://www.linkedin.com/in/alexlevy0)
- Twitter: [@alexlevy0](https://twitter.com/alexlevy0)


<div align="center">
<img src="https://github.com/fnky/fnky/raw/fnky/img/ie.jpg" alt="Best viewed with Microsoft Internet Explorer" align="center" width="128">
</div>
