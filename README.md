# knowledge-transfer

## Angular intro
##### Create simple 'html template driven' web form

#### 1. Workstation setup
  * (overall reference guide) https://angular.io/docs/ts/latest/cli-quickstart.html#!#devenv
  * install [node.js and npm](https://nodejs.org/en/download/)
  * install [VS Code](https://code.visualstudio.com/)
#### 2. Install cli
  * `npm install -g @angular/cli`
#### 3. Create new project
  * `ng new <project name>`
#### 4. Create form component
   * `ng g component form` (where 'form' is the name of your form component)
   *  Add form 'selector' tags to parent app.component.html which will demonstate how html can be shared across components. 
#### 5. Create model class
   * `ng g class customer`
   ~~~~
export class Customer {

constructor(
   public firstname: string,
   public lastname: string,
   public address: string,
   public address2: string,
   public email: string,
   public phonenumber?: string,  //question mark indicates field is optional
){ }

}
~~~~

   * create template driven form in html. 
