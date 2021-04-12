#Features
dropdown with multiple selction option
bind to any custom data source
search item with custom placeholder text
select/de-select items

#Installation

`npm install multiSelect`


And then include it in your module (see app.module.ts):

...

import { MultiSelectComponent } from './multi-select/multi-select.component';
// ...

@NgModule({
  declarations: [
    MultiSelectComponent
	// ...
  ]
  // ...
})
export class AppModule {}

...

Usage

...
import { CountryList } from './multi-select/country-list';
// ...


export class AppComponent {
  // ...
  countries = CountryList;
}

// ...
...

...
// ...
<multiSelect [options]="countries" [filter]="true" filterBy="label,value"></multiSelect>
// ...
...