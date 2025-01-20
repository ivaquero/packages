# German Work Time Sheet Template (Stundenzettel)

A Typst template for tracking work hours, designed for German-speaking contexts.

![Document preview](thumbnail.png)

## Usage:
```typst
#import "@preview/stundenzettel:0.1.0": timesheet

#timesheet(

name:"Lara Langname",
month: "Januar",
year: "2025",
csv.decode("
01.01.2025; Bugs suchen; 8; 42,00
02.01.2025; Bugs suchen; 8; 42,00
03.01.2025; 1st Level Support; 8; 42,00
04.01.2025; 2nd Level Support; 8; 42,00
05.01.2025; Typst Dokumente; 8; 42,00
", delimiter: ";").flatten(),
)
```