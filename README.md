# labuisimpfsappa2nodeauth_nt

## 1. Setting Up the infrastructure
### 4 Create and configure the Angular 2 project
```
cd labuisimpfsappa2nodeauth
git clone https://github.com/angular/quickstart.git frontend
```

## 2. Display Data in Angular 2
### 1 Create the component
 vscode preferences,add
 ```
 {
    "files.autoSave": "afterDelay",
    "typescript.check.tscVersion": false,
    "workbench.colorTheme": "Visual Studio Dark",
"files.exclude": {
    "**/*.js":true,
    "**/*js":{"when":"$(basename).ts"}
  }

}
```

## 3.
### 1
```
npm install --save @angular/material @angular/animations
```
```
'@angular/material':'npm:@angular/material/bundles/material.umd.js',
'@angular/animations': 'npm:@angular/animations/bundles/animations.umd.js'
```
 
 
### 3
KENG  
must add HttpModule in app.module.ts
```
'@angular/material':'npm:@angular/material/bundles/material.umd.js',
'@angular/animations': 'npm:@angular/animations/bundles/animations.umd.js'

import { NgModule }      from '@angular/core';
import { BrowserModule } from '@angular/platform-browser';
import {MaterialModule} from '@angular/material';
import { MessagesComponent} from './messages.component';
import { AppComponent }  from './app.component';
import {HttpModule} from '@angular/http';
import { WebService} from './web.service';

@NgModule({
  imports:      [ BrowserModule,MaterialModule,HttpModule ],
  declarations: [ AppComponent,MessagesComponent ],
  bootstrap:    [ AppComponent ],
  providers: [WebService]
})
export class AppModule { }
```
 

## 5. Creating a Form in Angular
### 1
must install typesctipt 2.2.2 in global and in project
```
npm install -g typescript@2.2.2 
npm install typescript@2.2.2 -D
```
