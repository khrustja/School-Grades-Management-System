# SchoolGradesMvcSite

Навчальний вебсайт на **ASP.NET Core MVC + SQLite + Identity** для системи управління шкільними оцінками.

## Що реалізовано
- базова MVC-архітектура: моделі, контролери, Razor Views;
- база даних SQLite;
- ролі доступу: **Guest**, **User**, **Administrator**;
- авторизація через **ASP.NET Core Identity**;
- вхід, вихід, зміна пароля, реєстрація через Identity;
- CRUD для учнів, предметів, вчителів, оцінок;
- призначення предметів вчителям;
- історія оцінок та середній бал учня;
- звіти: табель учня, рейтинг, статистика по класах, експорт CSV;
- адміністрування користувачів і ролей;
- імпорт і експорт учнів у CSV;
- **4 додаткові командні функції для окремих feature-гілок**.

## Додаткові командні функції
1. **Export Student Report to CSV** — експорт табеля конкретного учня в CSV.
2. **Filter Students by Class** — пошук і фільтрація списку учнів.
3. **View Top Student in Class** — визначення найкращого учня в обраному класі.
4. **Add Teacher Comment to Grade** — окрема сторінка редагування коментаря до оцінки.

## Ролі
- **Guest**: бачить головну, опис системи й предмети у режимі перегляду.
- **User**: працює з учнями, предметами, оцінками та звітами.
- **Administrator**: додатково керує вчителями, користувачами та доступом.

## Тестові акаунти
- `admin / admin123`
- `teacher / teacher123`

## Запуск
1. Встановити **.NET 8 SDK**.
2. Відкрити папку проєкту у Visual Studio 2022 або VS Code.
3. Виконати:
   ```bash
   dotnet restore
   dotnet run
   ```
4. Відкрити сайт за адресою, яку покаже консоль.

## CI/CD
У проєкті додані GitHub Actions workflow:
- `.github/workflows/ci.yml` — build + test
- `.github/workflows/cd.yml` — publish + artifact

## Документація
- `TEAM_BRANCH_PLAN.md` — розподіл 4 функцій по учасниках
- `docs/SRS_UPDATE_v1.1.md` — зміни до SRS
- `docs/UseCaseDiagram_v1.1.puml` — оновлена use case diagram
- `docs/ClassDiagram_Impact_v1.1.md` — чи вплинули зміни на class diagram
