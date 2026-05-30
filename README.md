# My-портфолио

Next.js + TypeScript портфолио для GitHub Pages.

## Что готово

- Главная страница с двумя областями.
- Левая колонка с информацией обо мне и sticky-поведением на desktop.
- Правая независимо прокручиваемая колонка с папками отраслей.
- Адаптивная mobile-версия без sticky.
- Страницы-заглушки отраслей.
- Базовые дизайн-токены: цвета, типографика, кнопки, карточки.

## Данные

Типы лежат в `src/data/types.ts`, отрасли — в `src/config/industries.ts`.

```ts
export type Industry = {
  slug: string;
  title: string;
  description?: string;
  coverImage?: string;
  projects: Project[];
};
```

## Изображения отраслей

Папки под будущие обложки:

- `public/industries/railway-transport`
- `public/industries/aviation`
- `public/industries/industry`
- `public/industries/research-and-concepts`

## Команды

```bash
npm install
npm run dev
npm run build
```

База данных не нужна: сайт можно собрать в статические файлы через `next build`.
