# Lern-Bericht
Adrian Bicskei

## Einleitung

Im LA_133_1005_SitzungsVerfolgung ging es darum bei einer Webapplikation mit einer Ablauf von 5 Seiten eine Sitzungsverfolgung mit JSF zu realisieren. 

## Was habe ich gelernt?

Bei diesem Lernauftrag habe ich gelernt, wie man Benutzereingaben während einer Sitzung im Controller speichert. 

## Beschreibung




Um eine Benutzereingabe während einer Sitzung im Controller zu speichern, muss man als erstes beim inputText Formularelement den Value an den controller weitergeben, wo es als String gespeichert wird. 


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

✍️ Erklären Sie kurz und bündig, inwiefern die von Ihnen verwendeten Medien zeigen, was Sie gelernt haben.

# Reflektion zum Arbeitsprozess

Gut gegangen ist die Benutzereingaben dem Controller weiterzugeben und diese speichern. 

Nicht gut gelaufen ist es den Session ID auszugeben. 

**VBV**: ✍️ Formulieren Sie davon ausgehend einen *handelbaren* Verbesserungsvorschlag.
