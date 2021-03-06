Accordion Sample Component
======

This content package contains a CQ accordion component based on Bootstrap. The package project was generated using the [simple-content-package-archetype](http://dev.day.com/docs/en/cq/current/core/how_to/how_to_use_the_vlttool/vlt-mavenplugin.html#simple-content-package-archetype).

Building
--------

This project uses Maven for building. Common commands:

From the project directory, run ``mvn -PautoInstallPackage clean install`` to build the bundle and content package and install to a CQ instance.

Try it
------

Navigate to [http://localhost:4502/cf#/content/bruce/accordion-demo.html](http://localhost:4502/cf#/content/bruce/accordion-demo.html) to view the component in edit mode.

Try [http://localhost:4502/content/bruce/accordion-demo.html?wcmmode=disabled](http://localhost:4502/content/bruce/accordion-demo.html?wcmmode=disabled) to see how it renders when WCMMode is disabled.

Using with VLT
--------------

To use vlt with this project, first build and install the package to your local CQ instance as described above. Then cd to `src/main/content/jcr_root` and run

    vlt --credentials admin:admin checkout -f ../META-INF/vault/filter.xml --force http://localhost:4502/crx

Once the working copy is created, you can use the normal ``vlt up`` and ``vlt ci`` commands.

Specifying CRX Host/Port
------------------------

The CRX host and port can be specified on the command line with:
mvn -Dcrx.host=otherhost -Dcrx.port=5502 <goals>

