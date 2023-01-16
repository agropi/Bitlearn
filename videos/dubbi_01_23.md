# Domande
## Ontologie
- nomenclatura ontologia (es. liot.livingiot.smartagri? oppure www.liot.org/ns/smartagri)
- formato file (ttl, rdf) e estensione (owl?rdf?)
- schema: urn o http?
- separatore della classe finale: # o . ? es. urn:liot:livingiot.smartagri#so2sensor  o urn:liot:livingiot.smartagri.so2sensor ?
- come si inserisce sensor/so2sensor? chiamando la classe sensor_so2sensor?
- gli individui vanno in un file separato che importa l'ontologia verticale. Quali? solo i sensori/attuatori, anche i valori?
-  altre ontologie: oltre a ssn (e sosa indirettamente), va importato  liot.org/ns/core? Sì
- usiamo i prefissi: sì nelle ontologie, anche nei jsonld?
- unità di misura: va usato qdt?  NO, unit-of-measure.org. Ad esempio, il grado  di temperatura è definito da
http://www.ontology-of-units-of-measure.org/resource/om-2/degree

## JSONLD
- la struttura del JSONLD deve avere graph in testa o può seguire la forma prevista nel cookbook 2.2 ?

## Registry
- le tag delle immagini devono avere la forma  liot-registry.living-iot.it:5001/sagr/airsensor ?
- che tag dare per far scaricare al bootloader una sola immagine per gestire device driver diversi?
- funzionano gli account sagr-001 e sccm-001 ?


## Configuratore
- ci sono già delle proprietà che ci interessano (es. urn:liot:livingiot.core.properties:AmbientTemperature) ma collegate a driver di shbh (es. drivers.ZwaveConnector)
Dobbiamo ricrearle _con un nome diverso_, usando possibilmente lo stesso tipo (es. um:degree) e connettendole al nuovo driver? Sì
