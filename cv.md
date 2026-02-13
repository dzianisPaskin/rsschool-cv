# Denis Paskin

[Wroclaw, Poland](https://maps.app.goo.gl/EXkrBqADwByiBF6n9) | [LinkedIn](https://www.linkedin.com/in/denis-paskin-a121b9220) | [Email](mailto:askin.denis.00@gmail.com) | [GitHub](https://github.com/dzianisPaskin)

Frontend developer with 3+ years of experience designing scalable web applications in E-commerce, Marketing, and Healthcare with React, Next.js, Typescript, and JavaScript. Write maintainable, clean, and test-driven code.

## Work experience

**Middle Frontend Developer at IAV GmbH (Andersen)** _01/2025 - 06/2025_

- Built an admin panel that centralizes project ticket data from platforms like Jira, providing detailed insights such as fill rates, statistics, and comparisons.
- **Contributions:**
  - Configured CI/CD and automated deployment to Rancher via Helm Charts, improving release efficiency.
  - Wrote unit and e2e tests, reducing potential bugs.
  - Implemented a cross-browser compatible UI, ensuring consistent performance across major browsers.
  - Led a team of two engineers by defining priorities and creating tasks, which helped accelerate and optimize development.
- **Tools:** TypeScript, React, Jotai, Ant Design, Emotion, Vite, Vitest, RTL, Cypress, TanStack Query, i18Next, Keycloak, Helm, Rancher, CI/CD, GitLab

**Middle Frontend Developer at Swiss-Commerce (Andersen)** _01/2024 - 12/2024_

- Developed an app for dropshippers that enables users to order goods from stock, choose suppliers, and set delivery terms or shipping companies.
- Developed a dashboard with a stock overview and a delivery management table, where users can track delivery status and details, adjust terms, and download delivery details as PDF files.
- **Contributions:**
  - Implemented accessibility guidelines (WCAG Level AA) and leveraged the M3 design system to create a more usable and user-friendly interface, which improved overall experience, earned positive customer feedback, and increased the number of users.
- **Tools:** TypeScript, Next.js, Redux Toolkit, React Hook Form, TanStack Query/Table, MSW, Storybook, MUI, Styled-components, Tailwind CSS, React Virtuoso, Jest, RTL, Cypress, Nx, i18Next, GitLab

**Junior Frontend Developer at Mariacher and Friends Werbeagentur GmbH (Andersen)** _07/2023 – 12/2023_

- Created a user-friendly hotel booking website that improved customer transactions by streamlining the booking process and enhancing user engagement.
- **Contributions:**
  - Refactored legacy code and optimized asset delivery by implementing Critical Rendering CSS, preload, and lazy loading, reducing load time from 7s to 4s and improving Core Web Vitals.
  - Implemented asset caching with Service Workers, resulting in improved page load speeds and enhanced user experience.
  - Applied semantic HTML and W3C patterns, which improved SEO metrics and accessibility.
- **Tools:** JavaScript, PHP, CSS, JQuery, WordPress, TYPO3

**Freelance** _07/2022 – 06/2023_

- Developed websites and landing pages using JavaScript, Typescript, jQuery, React, Bootstrap, CSS/SCSS, Gulp

## EDUCATION

**Vitebsk State University named after P.M. Masherov** _2014 - 2019_

- Bachelor's degree in Physical Education and Sports

## LANGUAGES

- English - B2
- Polish - A2
- Russian - Native

## SKILLS

**Hard:** JavaScript, TypeScript, React, Next.js, Redux, Redux Toolkit, Jotai, TanStack Query/Table, React Hook Form, Bootstrap, Styled-Components, Storybook, Webpack, Vite, Nx monorepo, Jest, RTL, Vitest, Cypress, MSW, Ant Design, Emotion, MUI, Tailwind CSS, CSS/SCSS modules, Docker, CI/CD, GitLab, HELM, Rancher, Gulp, TDD, SOLID, REST

**Soft:** Commitment, focus on qaulity and detail, mentoring and knowledge sharing, continuous learning and self-development, active collaborator within a team.

## Code example

```typescript
const towerBuilder = (nFloors: number): string[] => {
  const pyramid = [];
  const floorLegth = nFloors * 2 - 1;
  let floor = Array(floorLegth).fill("*").join("").split("");
  let emptySpaceStart = 0;
  let emptySpaceStartEnd = floorLegth - 1;
  pyramid[nFloors - 1] = floor.join("");

  for (let i = nFloors - 2; i >= 0; i--) {
    floor = floor.map((it, idx) => {
      if (idx === emptySpaceStart || idx === emptySpaceStartEnd) return " ";
      return it;
    });

    pyramid[i] = floor.join("");

    emptySpaceStart += 1;
    emptySpaceStartEnd -= 1;
  }

  return pyramid;
};
```
