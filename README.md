# veebiraamistikud2023

## Lingid

[Jaagup Tigu](https://tigu.hk.tlu.ee/~jaagup/23/)

## Kohtumine 09.09.2023
## kodutöö 1
Sisseloeteud andmestiku kujundamine veebilehel.
Vajadusel tehke tunni näitel uuesti läbi. Otsige koostage oma andmestik. Kuvage andmed lehele. Kui jaksu, siis katsetage osa andmete näitamist / peitmist. 

### Tervitus02.html

See sisaldab näiteid kahe funktsiooni kasutamise kohta ning lisaks sellele parameetrite props kasutuse kohta.
Jäi õhku küsimus, kas on võimalik props asendada ka mingi muu sõnaga?
näide:

```javascript

  <script type="text/babel">
     const root= ReactDOM.createRoot(document.getElementById("kiht1"))

    function Tervitus(props){
      return <h3>Tere, {props.eesnimi} {props.perenimi}!</h3>;
    }
    
    function Leht(){
      return (
        <div>
          <h1>Tervitusleht!</h1>
          
          <Tervitus eesnimi="Toivo" perenimi="Pärnpuu"/>
          <Tervitus eesnimi="Mari" perenimi="Tamm"/>
          <Tervitus eesnimi="Juhan" perenimi="Juurikas"/>
        </div>
      );
    }

     root.render(<Leht />);
  </script>

```

### Tervitus04.html

Tingimuse lisamine, kui andmete sisu on olemas kuva sisu, muu juhul näita, et sisu on puudu.
Kasutusel on Javascripti konstruktioon ternary operator ?"":"", mis on lühend if-else konstruktsioonile.

```javascript

    function Tervitus(props){
      return <h3>Tere, {props.eesnimi ? props.eesnimi: "eesnimi puudub"} {props.perenimi ? props.perenimi: "perenimi puudub"}!</h3>;
    }
  
```
