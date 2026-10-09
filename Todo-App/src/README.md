https://funet-my.sharepoint.com/:v:/g/personal/3ggyhmu26_svenjo_folkuniversitetet_nu/IQBGRxqmdGXPQ4PyfnvsZANWAbntN7sPyBX_ujipEFdoTuE?e=mFWNlf&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D

State‑hantering
svar:
med Reacts useState håller jag reda på uppgiftrena där jag lagrar en array med alla todos och uppdaterar den när något läggs till eller tas bort. 
Varje gång state ändras triggar React en omrendering, vilket gör att gränssnittet automatiskt visar den nya listan. 

Oföränderlighet (Immutability)
svar:
När jag tar bort en uppgift använder jag filter() som också returnerar en ny array. Detta gör att React kan se förändringen och uppdatera gränssnittet korrekt.

kodgranskningen

react kommer inte att omrendera med push

jsg skulle ha gjort så här 

function addTodo(todos, text) {
  return [...todos, text];
}

setTodos(prev => [...prev, text]);

Problemlösning & Reflektion (3–5 meningar)
svar: när jag körde fast titta jag vart problemet låg försöka förstå allt igen. Om jag inte lyckades lösa problemet själv så andvända jag mig av AI som fick hjälpa mig att först vad för fel jag hade gjort, och förklara hur och varför jag ska göra på ett visst sätt.