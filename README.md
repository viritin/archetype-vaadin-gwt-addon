# archetype-vaadin-gwt-addon

A project template for Vaadin add-ons that...

 * makes it easy to develop the add-on (UI tests in same module as the actual add-on)
 * makes OSGi compatible add-ons by default
 * emphasis testing: supports multiple UI tests with a searchable listing, setup for automated browser level testing
 * Supports GWT extensions, see [archetype-vaadin-addon](https://github.com/viritin/archetype-vaadin-addon) for a better one designed for server side compositions and JS only add-ons

## Using the archetype

Only snapshots are so far released, but you can use them with following CLI command:

    mvn org.apache.maven.plugins:maven-archetype-plugin:2.4:generate  \
        -DarchetypeGroupId=in.virit  \
        -DarchetypeArtifactId=archetype-vaadin-gwt-addon  \
        -DarchetypeRepository=https://oss.sonatype.org/content/repositories/snapshots/  \
        -DarchetypeVersion=2.0-SNAPSHOT

Maven will then prompt for group and archetype id for your project. If you are unsure what to give, use org.vaadin.addons for groupId and something derived from your add-on name, like *my-awesome-addon*.

Then see the README.md from the generated project for more instructions.

The archetype is quite new, so there is sure some rough edges left. Don't hesitate to report issues!
