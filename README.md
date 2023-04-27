# Appunti

Creare una cartella con cognome.nome.4H.Firstdb

Lanciare il visual studio code e aprire la cartella appena creata

Lanciare un terminale

Scrivere "dotnet new console"

Visual studio coce creera una cartella obj un csproject e un Program.cs

Aprire Program.cs

Ora dobbiamo cercare sulla rete chinook.db

Andare su Sqlitetutorial.net 

<a href = "https://www.sqlitetutorial.net/sqlite-sample-database/">

<img 
src="https://user-images.githubusercontent.com/116791222/234796021-8f259456-17dd-4b0b-bdc4-05b7243e69c4.png"
Width="600"
/>

</a>

il file da scaricare si trova nella sezione Download SQLite sample database

<img 
src="https://user-images.githubusercontent.com/116791222/234798006-06c01e35-cd3f-4772-ab83-5b305904634a.png"
/>

Installare il plugin per visual studio code che si chiama SQLite 

!!!!SQLite non è un database è una libreria!!!!!!!

Fare pulsante destro su chinook.db spostato in precedenza nella stessa cartella del progetto e cliccare "Open Databse"

Ora su program scrivere

<img 
src="https://user-images.githubusercontent.com/116791222/234799608-82c31ec5-3c56-4149-92a8-9f8beaa6bbd0.png"
/>

Ora entrare nel csproj e cercare "<PackageReference Include="sqlite-net-pc1" Version="1.8.116""

Quindi il nostro programma utilizza una libreria di nome "sqlite-net-pcl"

Se non è presente fare i seguenti passaggi
 
Ora copio il nome della libreria prima citata apro il terminale e scrivo "dotnet add package sqlite-net-pcl"

Adesso rientriamo nel Program e scrivere in cima "using SQLite"

Ora provare ad avviarlo

Per continuare scrivere il seguete comando

<img
src="https://user-images.githubusercontent.com/116791222/234801029-d85168ee-8ad6-41a8-8f0b-60c6fbe1a2a9.png"
/>

Ora si può notare che ci sarà un errore nella parola Artist, questo avviene perchè non abbiamo una classe di nome Artist

Quindi scrivere in fondo al programma:

public class Artist
{

}

Dopo questo il problema sembrera risolto, ma non avremo delle variabili all'interno della classe dove salvare i dati

Aggiungere quindi dentro la classe Artist queste cose:

public int ArtistId{get;set;}

public sting Name{get;set;}

