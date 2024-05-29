# Hi, I'm @resu 👋

## profile.ts

```typescript
import { Profile } from './profileTypes';

const resu: Profile = {
  availability: {
    timezone: "America/Los_Angeles",
    daysAvailable: ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"],
    workingHours: { start: "08:00", end: "17:00" },
    breakTime: { start: "12:00", end: "13:00" }
  },
  skills: {
    languages: ["C++", "JavaScript", "TypeScript", "Go", "Rust"],
    frameworks: ["React", "Node", "Vite", "Tauri"],
    frontend: ["MUI", "Tailwind", "Shadcn"],
    architecture: ["microservices", "cloud-native", "event-driven"],
    databases: ["PostgreSQL", "Redis"],
    devops: ["Prometheus", "Grafana", "GitHub Actions", "Docker", "K8s"],
    cloud: ["AWS", "Digital Ocean", "Cloudflare"]
  },
  workspace: {
    editor: "VSCode",
    theme: "Dracula",
    remote: true,
    fuelledBy: "☕"
  },
};
```

## profileTypes.ts

```typescript
interface Availability {
  timezone: string;
  daysAvailable: string[];
  workingHours: { start: string; end: string };
  breakTime: { start: string; end: string };
}

interface Skills {
  languages: string[];
  frameworks: string[];
  frontend: string[];
  architecture: string[];
  databases: string[];
  devops: string[];
  cloud: string[];
}

interface Workspace {
  editor: string;
  theme: string;
  remote: boolean;
  fuelledBy: string;
}

export interface Profile {
  availability: Availability;
  skills: Skills;
  workspace: Workspace;
}
```
