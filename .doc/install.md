### Installation Instruction 
[refrance link](https://www.djamware.com/post/5be52ce280aca72b942e31bc/ionic-4-angular-7-and-cordova-tutorial-build-crud-mobile-apps)\
[Repo link](https://github.com/didinj/ionic4-angular7-example.git)
1. create app

```bash
    $ ionic start cultureapp --type=angular
```

2. if any dependency is missing and permission error 

```bash
    $ sudo npm i --unsafe-perm
```
3. Add and install Ionic lab for emulator testing

```bash
    $ npm install --save-dev @ionic/lab
```

4. Run Application in Lab

```bash
    $ ionic serve -l
```

5. if you want to add Angular 7 Material and CDK

```bash
    $ ng add @angular/material
```
 -----------------------------------------------
 - Type enter or yes for every question that showed up.

 ```bash
    ? Choose a prebuilt theme name, or "custom" for a custom theme: Indigo/Pink
    [ Preview: https://material.angular.io?theme=indigo-pink ]
    ? Set up HammerJS for gesture recognition? Yes
    ? Set up browser animations for Angular Material? Yes
 ```     
- Next, register all required Angular Material components or modules to `app.module.ts`. Open and edit that file then add this imports.

```bash
    import {
    MatInputModule,
    MatPaginatorModule,
    MatProgressSpinnerModule,
    MatSortModule,
    MatTableModule,
    MatIconModule,
    MatButtonModule,
    MatCardModule,
    MatFormFieldModule } from "@angular/material";
    import { DragDropModule } from '@angular/cdk/drag-drop';
    import { ScrollingModule } from '@angular/cdk/scrolling';
```
- Register the above modules to `@NgModule` imports.

```bash
    imports: [
        BrowserModule,
        IonicModule.forRoot(),
        AppRoutingModule,
        BrowserAnimationsModule,
        DragDropModule,
        ScrollingModule,
        MatInputModule,
        MatPaginatorModule,
        MatProgressSpinnerModule,
        MatSortModule,
        MatTableModule,
        MatIconModule,
        MatButtonModule,
        MatCardModule,
        MatFormFieldModule
    ],
```

