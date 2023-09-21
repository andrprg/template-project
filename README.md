#Настройки

Установим angular-eslint
ng add @angular-eslint/schematics

Устанавливаем Prettier
npm install prettier --save-dev

Создадим файл .prettierrc и добавим в него
{
  "bracketSpacing": true,
  "printWidth": 140,
  "semi": true,
  "singleQuote": true,
  "tabWidth": 2,
  "useTabs": false
}

Создадим .prettierignore и добавим в него
# Add files here to ignore them from prettier formatting
/dist
/coverage
/tmp
/node_modules
/nginx
/.vscode
/.idea
package-lock.json
package.json
yarn.lock

Запуск линтера
ng lint --fix

Добавим Angular material
ng add @angular/material

Все стили из папки theme добавляем как import в файл style.scss

Добавим в angular.json свойство
"@schematics/angular:component": {
  "style": "scss",
  "changeDetection": "OnPush"
},

Также на уровне базового компонента (AppComponent), добавим changeDetection
@Component({
  selector: 'app-root',
  templateUrl: './app.component.html',
  styleUrls: ['./app.component.scss'],
  changeDetection: ChangeDetectionStrategy.OnPush,
})


# TemplateProject

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 16.2.3.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.


