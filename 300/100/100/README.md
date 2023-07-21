# 100 - React Component (Client-side)

The following creates a component named ```apps/to-do``` using a component generator, provided by a react env. It sets ```my-org.tasks-scope``` as its scope name.

```
$ bit create react apps/to-do --scope my-org.tasks-scope --aspect teambit.react/react-env
```

Command synopsis:

```
$ bit create TEMPLATE_NAME COMPONENT_NAMES... --namespace STRING --scope STRING --aspect STRING --template STRING --path STRING --env STRING
```

The output is similar to the following:

```
1 component(s) were created

my-org.tasks-scope.apps/to-do
location: tasks-scope/apps/to-do
env: teambit.react/react-env (set by template)
```

env configuration is according to workspace variants, template config or --env flag. learn more at https://bit.dev/docs/envs/using-envs

This component has a **component ID**: ``my-org.tasks-scope/apps/to-do``. This ID consists of the component's scope name and component name. Component IDs are used by workspaces and scopes to reference components.

This components also has a **development environment**, or 'env'. An env is a also a component. It provides this component with pre-defined configuration and a set of development tools such as a compiler (```bit compile apps/to-do```), a tester (```bit test apps/to-do```), a linter (```bit lint apps/to-do```), and more. Envs can be of different types. This component was configured (by the 'react-env' component generator) to use the [React env](https://bit.dev/docs/react-env/set-up-your-env) (teambit.react/react).

*Note*: the component used for this demo is not identical to the one created in your workspace. The implementation for this component can be copied from the editor down below.

## 100 - Component Files

A component can be of different types. A NodeJS module, an Angular component, a CSS module, and so on. Since this component was created by the react template, the generated files are for a React component.

These files include standard React implementation files, as well as development files that are handled by the different tools ('env services') which are provided by the React env.

To learn about **compiling**, **testing**, **documenting**, rendering components in isolation ('**compositions**'), as well as other development procedures, see [Running env services](https://bit.dev/docs/getting-started/composing/dev-environments#running-env-services).

Head over to the workspace UI (http://localhost:3000/), to further explore the component (run bit start to run the UI server).

## 200 - Component configuration and metadata

see https://bit.dev/docs/getting-started/composing/creating-components?component_type=0

WE ARE HERE ...
