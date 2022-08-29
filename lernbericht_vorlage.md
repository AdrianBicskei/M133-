# Lern-Bericht
Adrian Bicskei

## Einleitung

Im LA_133_1005_SitzungsVerfolgung ging es darum bei einer Webapplikation mit einem Ablauf von 5 Seiten eine Sitzungsverfolgung mit JSF zu realisieren. 

## Was habe ich gelernt?

Bei diesem Lernauftrag habe ich gelernt, wie man Benutzereingaben während einer Sitzung im Controller speichert. 

## Beschreibung

Um eine Benutzereingabe während einer Sitzung im Controller zu speichern, muss man als Erstes beim inputText Formularelement den Value an den Controller weitergeben, wo es als String gespeichert wird. 


Benutzereingabe durch Formularfeld
```
 <h:outputLabel for="eingabe" value="Ihr Name: "/> 
 <h:inputText value="#{helloManagedBean.name}" id="name"/>
```           
            
Speicherung im Controller            
```            
private String name;
            
public String getName() {
  return name;
}

public void setName(String name) {
  this.name = name;
}
```            

![ezgif com-gif-maker](https://user-images.githubusercontent.com/112397931/187230011-9f822a45-a830-4700-a16d-0de89ea49e40.gif)

## Verifikation

In der zweiten Zeile der XHTML code ist zu sehen, wie der Benutzereingabe an den Controller übergeben wird.
In der Java Code ist zu sehen, wie dieser Eingabe als String im Controller gespeichert wird.

# Reflektion zum Arbeitsprozess

Gut gegangen ist es, die an den Controller weitergegebenen Benutzereingaben zu speichern. 

Nicht gut gelaufen ist es aufgrund Syntaxfehler, die Benutzereingaben dem Controller weiterzugeben und diese speichern. 

**VBV**: Damit ich das nächste Mal nicht Schwierigkeiten bei der Weitergabe der Benutzereingaben an den Controller habe, werde ich auf die Syntax besser achten. 
