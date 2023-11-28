# Eclipse EMF Services

EMF Services provides libraries that extend the core EMF framework with additional services or more powerful versions of services provided by EMF itself.

The project currently provides three components:

* [EMF Validation](https://github.com/eclipse-emfservices/emf-validation), which extends the core validation support of EMF itself with constraint definitions, customizable model traversal algorithms, constraint parsing for languages, configurable application-specific validation contexts, and validation listeners.
* [EMF Transaction](https://github.com/eclipse-emfservices/emf-transaction), which provides transactional semantics for (local) EMF model changes, with support for multi-threading, model integrity, batched events, and automatic undo/redo support. The framework also features improved integration between EMF and Eclipse, with traceability between EMF models and workspace resources, and integration with the Eclipse jobs API and the Eclipse operation history.
* [EMF Query](https://github.com/eclipse-emfservices/emf-query) provides a Java API to define semi-declarative queries on EMF models and execute them. *This component is no longer maintained.*

Each component is developped and released separately, although typically there is a synchronized major release each year, for the Eclipse Simultaneous Release.

The project is open for proposal for other components as long as:

* they are domain-agnostic and could be usefull to several other modeling projects (at Eclipse or elsewhere);
* they are reasonably small and self-contained (minimum dependencies beyond EMF and "core" Eclipse projects);
* the component includes comprehensive tests and non regression strategy;
* someone is ready to support and maintain them on the long term.
