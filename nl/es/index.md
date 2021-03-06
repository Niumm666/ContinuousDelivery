---

copyright:
  years: 2015, 2017
lastupdated: "2017-5-19"

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Iniciación a la entrega continua
{: #cd_getting_started}

Puede adoptar un enfoque DevOps mediante {{site.data.keyword.contdelivery_full}}, que incluye cadenas de herramientas abiertas que automatizan la creación y despliegue de aplicaciones. Puede empezar creando una sencilla cadena de herramientas que dé soporte a las tareas de desarrollo, despliegue y operaciones.
{: shortdesc}

Después de crear una instancia de {{site.data.keyword.contdelivery_short}} seleccionándola en el catálogo de {{site.data.keyword.Bluemix_notm}}, puede elegir cómo desea empezar a trabajar con el servicio.
 ![Página de bienvenida de entrega continua](images/cd_landing_page.png)

* Para empezar a trabajar y a desplegar rápidamente la aplicación utilizando un conducto automatizado, en la sección "Inicio con un conducto" pulse **[Empezar aquí](#starting_with_a_pipeline)**. Luego podrá añadir más herramientas.
* Para crear y configurar una cadena de herramientas de entrega continua a partir de una plantilla, en la sección "Inicio desde una plantilla de cadena de herramientas" pulse **[Empezar aquí](#starting_from_a_toolchain_template)**. La cadena de herramientas integra herramientas para la planificación, despliegue de conductos y gestión de aplicaciones. Siempre puede añadir o eliminar herramientas de sus cadenas de herramientas.
* Si ya tiene cadenas de herramientas, en la sección "Inicio desde una plantilla de cadena de herramientas" pulse **Ver sus cadenas de herramientas**. Para obtener más información sobre cómo trabajar con cadenas de herramientas, consulte el apartado sobre [Utilización de cadenas de herramientas](/docs/services/ContinuousDelivery/toolchains_using.html){: new_window}.

**Consejo**: Los conductos se gestionan mediante cadenas de herramientas. Puede añadir un conducto a una cadena de herramientas existente. Si crea un conducto y no dispone de ninguna cadena de herramientas, se crea automáticamente una cadena de herramientas con un nombre predeterminado. Con la cadena de herramientas, puede ampliar las prestaciones del conducto integrándolo con otras herramientas y servicios.

##Visión
general de {{site.data.keyword.contdelivery_short}}
{: #cd_overview}

Con {{site.data.keyword.contdelivery_short}} puede crear, probar y entregar aplicaciones mediante las herramientas más utilizadas de la industria y prácticas de DevOps.
{:shortdesc}

El servicio {{site.data.keyword.contdelivery_short}} da soporte a los flujos de trabajo de DevOps:

 * Puede crear [cadenas de herramientas](/docs/services/ContinuousDelivery/toolchains_about.html){: new_window} abiertas integradas de DevOps para habilitar las integraciones de herramientas que dan soporte a las tareas de desarrollo, despliegue y operaciones.

  Una cadena de herramientas es un conjunto integrado de herramientas que sirve para desarrollar, crear, desplegar, probar y gestionar aplicaciones para repetir estas operaciones de forma cíclica de forma que se fácil gestionarlas. Las cadenas de herramientas pueden incluir herramientas de código abierto, servicios {{site.data.keyword.Bluemix_notm}} como [{{site.data.keyword.DRA_full}}](/docs/services/ContinuousDelivery/di_working.html){: new_window} y herramientas de terceros como GitHub, PagerDuty o Slack. 

 * Entrega continua mediante [conductos](/docs/services/ContinuousDelivery/pipeline_about.html){: new_window} automatizados.

  Automatice compilaciones, pruebas de unidad, despliegues y más. Cree, pruebe y despliegue de manera repetitiva con una mínima intervención humana. Esté listo para pasar a producción en cualquier momento.

 * Edite y envíe el código desde cualquier lugar utilizando el [IDE basado en web](/docs/services/ContinuousDelivery/web_ide.html){: new_window}.

  Cree, edite, ejecute, depure y complete tareas de control de código fuente en GitHub. Puede pasar fácilmente de editar el código a desplegarlo en producción. 
  
 * Colabore con su equipo y gestione su código fuentes con [Git Repository and Issue Tracker](/docs/services/ContinuousDelivery/git_working.html#git_working){: new_window} alojado en IBM y que se basa en GitLab Community Edition.

  Gestione repositorios Git a través de controles de acceso precisos que mantienen el código seguro. Revise el código y mejore la colaboración mediante solicitudes de fusión. Realice un seguimiento de los problemas y comparta ideas mediante el rastreador de problemas. Documente sus proyectos con un sistema wiki.

##Inicio con un conducto
{: #starting_with_a_pipeline}

Los conductos automatizan las compilaciones, despliegues y más. Para empezar con un conducto automatizado, seleccione una plantilla y especifique la ubicación del repositorio GitHub (repositorio).

Para [crear un conducto ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](https://console.bluemix.net/devops/pipelines/dashboard/create){:new_window} configurado para desplegar una aplicación Cloud Foundry, siga estos pasos:

1. Pulse **Cloud Foundry**.
1. Si desea utilizar otro nombre para el conducto, cambie el nombre predeterminado. El nombre del conducto lo identifica en {{site.data.keyword.Bluemix_notm}}.
1. Si desea utilizar otro nombre para la aplicación, cambie el nombre predeterminado. El nombre de la aplicación la identifica en {{site.data.keyword.Bluemix_notm}}. Este es el nombre de la aplicación en la que se despliega el conducto.
1. Si no tiene una cadena de herramientas, se crea automáticamente una cadena de herramientas con un nombre predeterminado. Si desea utilizar otro nombre para la cadena de herramientas, cámbiele el nombre. Los conductos se gestionan mediante cadenas de herramientas. Con la cadena de herramientas, puede ampliar las prestaciones del conducto integrándolo con otras herramientas y servicios.

 **Consejo**: Los conductos y las cadenas de herramientas pertenecen a las organizaciones (orgs). Si pertenece a una org que tiene cadenas de herramientas, puede utilizar dichas cadenas de herramientas aunque no las haya creado.

1. Seleccione la cadena de herramientas que desea utilizar o escriba un nombre para la nueva cadena de herramientas que desea crear.
1. Seleccione el proveedor de Git.

 **Sugerencia**: Si {{site.data.keyword.Bluemix_notm}} no está autorizado a acceder a su cuenta de GitHub, se le solicitará que pulse **Autorizar** para ir al sitio web de GitHub. Si no tiene ninguna sesión de GitHub activa, se le solicitará que inicie sesión. Pulse **Autorizar aplicación** para permitir que {{site.data.keyword.Bluemix_notm}} acceda a su cuenta de GitHub. 

 Si no está autorizado a acceder al repositorio {{site.data.keyword.ghe_short}}, alguien que tenga privilegios de administrador para el repositorio debe añadirle. Para obtener instrucciones sobre la autorización con {{site.data.keyword.Bluemix_notm}} dedicado para {{site.data.keyword.ghe_short}}, consulte [Iniciación a {{site.data.keyword.Bluemix_notm}} dedicado para {{site.data.keyword.ghe_short}}](/docs/services/ghededicated/index.html){: new_window}. Si necesita autorizar con su propia versión gestionada de {{site.data.keyword.ghe_short}}, siga los procedimientos internos.

    * Si tiene un repositorio y desea utilizarlo, seleccione **Enlazar** para el tipo de repositorio. Busque la ubicación del repositorio o seleccione el repositorio en la lista de repositorios disponibles.

    * Si desea crear un repositorio vacío, seleccione **Nuevo** para el tipo de repositorio. Escriba un nombre para el repositorio.

    * Si desea crear un clon de un repositorio, seleccione **Copiar** para el tipo de repositorio. Busque la ubicación del repositorio o seleccione el repositorio en la lista de repositorios disponibles.

    * Si desea bifurcar un repositorio de forma que pueda aportar cambios a través de solicitudes de extracción, seleccione **Bifurcar**. Busque la ubicación del repositorio o seleccione el repositorio en la lista de repositorios disponibles.

1. Seleccione un repositorio o especifique un URL de repositorio.
1. Pulse **Crear**. El conducto se crea, se configura y se visualiza en la página Visión general de la cadena de herramientas.
 ![Tarjeta de conducto](images/cd_pipeline.png)

Para crear un [conducto vacío ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](https://console.bluemix.net/devops/pipelines/dashboard/create){: new_window} sin etapas preconfiguradas:

1. Pulse **Personalizado**.
1. Si desea utilizar otro nombre para el conducto, cambie el nombre predeterminado. El nombre del conducto lo identifica en {{site.data.keyword.Bluemix_notm}}.
1. Si no tiene una cadena de herramientas, se crea automáticamente una cadena de herramientas con un nombre predeterminado. Si desea utilizar otro nombre para la cadena de herramientas, cámbiele el nombre. Los conductos se gestionan mediante cadenas de herramientas. Con la cadena de herramientas, puede ampliar las prestaciones del conducto integrándolo con otras herramientas y servicios.
1. Seleccione la cadena de herramientas que desea utilizar o escriba un nombre para la nueva cadena de herramientas que desea crear.
1. Pulse **Crear**. Se crea un conducto vacío y se representa como una tarjeta en la página Visión general de la cadena de herramientas.

##Inicio desde una plantilla de cadena de herramientas
{: #starting_from_a_toolchain_template}

Para crear y configurar una cadena de herramientas de entrega continua desde una [plantilla ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](https://console.bluemix.net/devops/create){: new_window}:

1. En la página **Crear una cadena de herramientas**, pulse una plantilla de cadena de herramientas.
1. Revise el diagrama de la cadena de herramientas que se dispone a crear. El diagrama muestra cada integración de herramientas en la fase del ciclo de vida correspondiente en la cadena de herramientas.

 **Consejo**: Algunas de las plantillas de cadena de herramientas tienen varias instancias de una integración de herramientas. Por ejemplo, la plantilla de la cadena de herramientas de microservicios de {{site.data.keyword.Bluemix_notm}} público contiene tres instancias de GitHub y tres instancias de Delivery Pipeline, una para cada uno de los tres microservicios.

 El diagrama de la imagen siguiente es un ejemplo. Cuando cree una cadena de herramientas, el diagrama mostrará cada integración de herramientas que forma parte de la cadena de herramientas.
 ![Diagrama_cadena_herramientas](images/toolchain_diagram.png)
1. Revise la información predeterminada para la configuración de la cadena de herramientas. El nombre de la cadena de herramientas la identifica en {{site.data.keyword.Bluemix_notm}}. Si desea utilizar otro nombre, cambie el nombre de la cadena de herramientas.
1. En la sección Integraciones de herramientas, seleccione las integraciones de herramientas que desee configurar para su cadena de herramientas. Algunas integraciones de herramientas no necesitan configuración. Para obtener información sobre cómo configurar las integraciones de herramientas, consulte [Configurar integraciones de herramientas](/docs/services/ContinuousDelivery/toolchains_integrations.html){: new_window}.
1. Pulse **Crear**. Para configurar la cadena de herramientas, se ejecutan varios pasos automáticamente. Las integraciones de herramientas que se configuran varían en función de la plantilla de cadena de herramientas que haya seleccionado y de si utiliza {{site.data.keyword.Bluemix_notm}} público o {{site.data.keyword.Bluemix_notm}} dedicado. Por ejemplo, si crea una cadena de herramientas de microservicios en {{site.data.keyword.Bluemix_notm}} público, se ejecutan estos pasos:

 * Se crea la cadena de herramientas.
 * Si ha configurado Delivery Pipeline, los conductos se crean y se activan.
 * Si ha configurado Sauce Labs, la cadena de herramientas se configura para añadir trabajos de prueba de Sauce Labs a los conductos.
 * Si ha configurado PagerDuty, la cadena de herramientas se configura para enviar notificaciones de alerta al servicio de PagerDuty que ha especificado.
 * Si ha configurado Slack, la cadena de herramientas se configura para enviar notificaciones sobre el estado de despliegue al canal Slack que ha especificado.
 * Si ha configurado la integración de una herramienta de código fuente como GitHub, el repositorio de ejemplo de GitHub se clona en su cuenta de GitHub.
