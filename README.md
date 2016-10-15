# 0DomacaZadaca
# JMBAG
{ 0036494891 }

{ 1. }
{ Primjećujem da postoje dvije nove datoteke ClassLibrary1.dll 
i ClassLibrary1.pdb i ako izbrišem datoteku ClassLibrary1.dll aplikacija
mi neće raditi ispravno. Naime datoteka ClassLibrary1.dll služi za dinamičko
povezvinje biblioteka i ako se ona ne nalazi unutar foldera tada aplikacija ne
može doprijeti do klase a time i same metode što uzrokuje poteškoće u radu.
Kad bih nekom morao poslati aplikaciju i ako želim da ta aplikacija normalno
radi tada moram poslati datoteke sa nastavkom .exe i .dll. }

{ 2. }
{ Aplikacija je koristila staru verziju asemblija zbog toga što prevodioc nije
preveo novu verziju projekta pa se u folderu i dalje nalaze datoteke od prijašnjeg 
prevođenja. Iz tog razloga se ispisuje stari string na ekran. }

{ 3. }
{ Ispisalo se Pero: Hello World. }

{ 4. }
{ Primjećujem da je dodana datoteka PeroClassLibrary.dll. }

{ 5. }
{ Aplikacija i dalje radi zato što sada koristimo metodu iz PeroClassLibrary a ne
iz one prve reference. Build i dalje radi zato što se PeroClassLibrary ne nalazi u
solutionu. }

{ 6. }
{ Build proces se ponašao kao i inače zato što je dohvaćanje NuGet paketa integrirano
u build proces, a u packages direktorij je vračen paket NodeTime. }
