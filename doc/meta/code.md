# Coding Styleguide

Die Coding Guidlines sind unbeding einzuhalten. Es wird noch nach einer Software
gesucht die diese überprüft und die Einhaltung erzwingt.

## Header Files

Include Guards sind in allen header files Pflicht. Dabei nutzten wir die
Kombination aus den guten alten ifndef-Guards sowie dem von Microsoft genutztem
pragma once

    #pragma once
    #ifndef COOL_CLASS_NAME_H__
    #define COOL_CLASS_NAME_H__

    ....

    #endif // include guard

## Allgemein

Alle Namen sind in CamelCase zu halten. Methoden, Funktionen und Variablen beginnen
dabei mit einem kleinen Buchstaben, Klassen immer mit einem Großbuchstaben.

Zur Einrückung werden 4 Spaces genutzt.

Öffnende geschweifte Klammern hinter Klassen und Methoden sind in die nächste
Zeile zu setzen. Bei *if*, *switch*, und Schleifen gehören diese in der selbe Zeile.

If-Konstruke ohne geschweifet Klammen sind immer unzulässig.

    class CoolClass
    {
    public:
        void methodName(type name, type anotherName)
        {
            if (name == anotherName) {

            }
        }
    };
