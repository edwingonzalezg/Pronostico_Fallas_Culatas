# Project Charter

## Business background

* El cliente es una empresa dedicada al transporte y la logística de hidrocarburos, que lidera el segmento Midstream en la cadena del petróleo de Colombia. Es una de las empresas más grandes del país por cantidad de activos y se encuentra entre las 10 compañías más grandes por ingresos operacionales y utilidades del país. Esta empresa cuenta con cerca de 9.000 kilómetros de oleoductos y poliductos por los que se transporta la mayoría del crudo y los refinados de Colombia.

![image](https://user-images.githubusercontent.com/119147133/204162874-d50a37e0-d06b-47d0-9a69-eea706b88aa2.png)

* La confiabilidad de las redes de transporte de hidrocarburos está directamente asociada al funcionamiento de las estaciones de bombeo. En Colombia, los sistemas de transporte de hidrocarburos operan en serie de estación a estación. De esta manera, el número y potencia hidráulica están en función del volumen a transportar, de la viscosidad del crudo, del diámetro de la tubería, de la resistencia mecánica y las condiciones geográficas. Las estaciones de bombeo de la red de hidrocarburos en Colombia operan en su mayoría a través de motores de combustión interna o eléctricos de alta potencia los cuales son los encargados de transmitir la potencia mecánica a la bomba la cual a su vez se encarga de impulsar el fluido (crudo) a través del oleoducto. Se requieren alternativas de tecnología de motores para operar al menor costo posible pero que sean capaces de satisfacer la demanda operando dentro los parámetros mínimos de emisiones de CO2 al ambiente. Teniendo en cuenta lo anterior y visualizando la importancia del negocio de petróleo para Colombia es necesario “garantizar la mayor producción de crudo al menor costo posible” para obtener la "mayor rentabilidad" posible en este sector y así generar una mayor contribución al país.

![image](https://user-images.githubusercontent.com/119147133/204162958-31eafc11-9cce-4919-89a4-30da454b3220.png)

* Actualmente uno de los principales problemas de las transportadoras de petróleo en Colombia son sus elevados costos debido a la alta cantidad de fallas que se presentan en sus estaciones. Por ejemplo, una de las principales transportadoras la cual nos reservamos el nombre, tiene un promedio de USD4.000.000 en costos anuales asociados a fallas. En la siguiente imagen se puede apreciar el comportamiento de los costos en mantenimiento:

![image](https://user-images.githubusercontent.com/119147133/204163100-4f14bdb8-f653-4a47-9806-599052e751d0.png)


## Scope
* What data science solutions are we trying to build?
* What will we do?
* How is it going to be consumed by the customer?

## Personnel
* Who are on this project:
	* Microsoft:
		* Project lead
		* PM
		* Data scientist(s)
		* Account manager
	* Client:
		* Data administrator
		* Business contact
	
## Metrics
* What are the qualitative objectives? (e.g. reduce user churn)
* What is a quantifiable metric  (e.g. reduce the fraction of users with 4-week inactivity)
* Quantify what improvement in the values of the metrics are useful for the customer scenario (e.g. reduce the  fraction of users with 4-week inactivity by 20%) 
* What is the baseline (current) value of the metric? (e.g. current fraction of users with 4-week inactivity = 60%)
* How will we measure the metric? (e.g. A/B test on a specified subset for a specified period; or comparison of performance after implementation to baseline)

## Plan
* Phases (milestones), timeline, short description of what we'll do in each phase.

## Architecture
* Data
  * What data do we expect? Raw data in the customer data sources (e.g. on-prem files, SQL, on-prem Hadoop etc.)
* Data movement from on-prem to Azure using ADF or other data movement tools (Azcopy, EventHub etc.) to move either
  * all the data, 
  * after some pre-aggregation on-prem,
  * Sampled data enough for modeling 

* What tools and data storage/analytics resources will be used in the solution e.g.,
  * ASA for stream aggregation
  * HDI/Hive/R/Python for feature construction, aggregation and sampling
  * AzureML for modeling and web service operationalization
* How will the score or operationalized web service(s) (RRS and/or BES) be consumed in the business workflow of the customer? If applicable, write down pseudo code for the APIs of the web service calls.
  * How will the customer use the model results to make decisions
  * Data movement pipeline in production
  * Make a 1 slide diagram showing the end to end data flow and decision architecture
    * If there is a substantial change in the customer's business workflow, make a before/after diagram showing the data flow.

## Communication
* How will we keep in touch? Weekly meetings?
* Who are the contact persons on both sides?
