## API Report File for "@backstage-community/plugin-azure-devops"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts
import { AnyApiFactory } from '@backstage/core-plugin-api';
import { AnyRouteRefParams } from '@backstage/frontend-plugin-api';
import { ConfigurableExtensionDataRef } from '@backstage/frontend-plugin-api';
import { Entity } from '@backstage/catalog-model';
import { ExtensionDefinition } from '@backstage/frontend-plugin-api';
import { FrontendPlugin } from '@backstage/frontend-plugin-api';
import { default as React_2 } from 'react';
import { RouteRef } from '@backstage/frontend-plugin-api';

// @alpha (undocumented)
const _default: FrontendPlugin<
  {},
  {},
  {
    'api:azure-devops': ExtensionDefinition<{
      kind: 'api';
      name: undefined;
      config: {};
      configInput: {};
      output: ConfigurableExtensionDataRef<
        AnyApiFactory,
        'core.api.factory',
        {}
      >;
      inputs: {};
      params: {
        factory: AnyApiFactory;
      };
    }>;
    'page:azure-devops': ExtensionDefinition<{
      kind: 'page';
      name: undefined;
      config: {
        path: string | undefined;
      };
      configInput: {
        path?: string | undefined;
      };
      output:
        | ConfigurableExtensionDataRef<
            React_2.JSX.Element,
            'core.reactElement',
            {}
          >
        | ConfigurableExtensionDataRef<string, 'core.routing.path', {}>
        | ConfigurableExtensionDataRef<
            RouteRef<AnyRouteRefParams>,
            'core.routing.ref',
            {
              optional: true;
            }
          >;
      inputs: {};
      params: {
        defaultPath: string;
        loader: () => Promise<JSX.Element>;
        routeRef?: RouteRef<AnyRouteRefParams> | undefined;
      };
    }>;
    'entity-content:azure-devops/pipelines': ExtensionDefinition<{
      kind: 'entity-content';
      name: 'pipelines';
      config: {
        path: string | undefined;
        title: string | undefined;
        filter: string | undefined;
      };
      configInput: {
        filter?: string | undefined;
        title?: string | undefined;
        path?: string | undefined;
      };
      output:
        | ConfigurableExtensionDataRef<
            React_2.JSX.Element,
            'core.reactElement',
            {}
          >
        | ConfigurableExtensionDataRef<string, 'core.routing.path', {}>
        | ConfigurableExtensionDataRef<
            RouteRef<AnyRouteRefParams>,
            'core.routing.ref',
            {
              optional: true;
            }
          >
        | ConfigurableExtensionDataRef<
            string,
            'catalog.entity-content-title',
            {}
          >
        | ConfigurableExtensionDataRef<
            (entity: Entity) => boolean,
            'catalog.entity-filter-function',
            {
              optional: true;
            }
          >
        | ConfigurableExtensionDataRef<
            string,
            'catalog.entity-filter-expression',
            {
              optional: true;
            }
          >;
      inputs: {};
      params: {
        loader: () => Promise<JSX.Element>;
        defaultPath: string;
        defaultTitle: string;
        routeRef?: RouteRef<AnyRouteRefParams> | undefined;
        filter?: string | ((entity: Entity) => boolean) | undefined;
      };
    }>;
    'entity-content:azure-devops/git-tags': ExtensionDefinition<{
      kind: 'entity-content';
      name: 'git-tags';
      config: {
        path: string | undefined;
        title: string | undefined;
        filter: string | undefined;
      };
      configInput: {
        filter?: string | undefined;
        title?: string | undefined;
        path?: string | undefined;
      };
      output:
        | ConfigurableExtensionDataRef<
            React_2.JSX.Element,
            'core.reactElement',
            {}
          >
        | ConfigurableExtensionDataRef<string, 'core.routing.path', {}>
        | ConfigurableExtensionDataRef<
            RouteRef<AnyRouteRefParams>,
            'core.routing.ref',
            {
              optional: true;
            }
          >
        | ConfigurableExtensionDataRef<
            string,
            'catalog.entity-content-title',
            {}
          >
        | ConfigurableExtensionDataRef<
            (entity: Entity) => boolean,
            'catalog.entity-filter-function',
            {
              optional: true;
            }
          >
        | ConfigurableExtensionDataRef<
            string,
            'catalog.entity-filter-expression',
            {
              optional: true;
            }
          >;
      inputs: {};
      params: {
        loader: () => Promise<JSX.Element>;
        defaultPath: string;
        defaultTitle: string;
        routeRef?: RouteRef<AnyRouteRefParams> | undefined;
        filter?: string | ((entity: Entity) => boolean) | undefined;
      };
    }>;
    'entity-content:azure-devops/pull-requests': ExtensionDefinition<{
      kind: 'entity-content';
      name: 'pull-requests';
      config: {
        path: string | undefined;
        title: string | undefined;
        filter: string | undefined;
      };
      configInput: {
        filter?: string | undefined;
        title?: string | undefined;
        path?: string | undefined;
      };
      output:
        | ConfigurableExtensionDataRef<
            React_2.JSX.Element,
            'core.reactElement',
            {}
          >
        | ConfigurableExtensionDataRef<string, 'core.routing.path', {}>
        | ConfigurableExtensionDataRef<
            RouteRef<AnyRouteRefParams>,
            'core.routing.ref',
            {
              optional: true;
            }
          >
        | ConfigurableExtensionDataRef<
            string,
            'catalog.entity-content-title',
            {}
          >
        | ConfigurableExtensionDataRef<
            (entity: Entity) => boolean,
            'catalog.entity-filter-function',
            {
              optional: true;
            }
          >
        | ConfigurableExtensionDataRef<
            string,
            'catalog.entity-filter-expression',
            {
              optional: true;
            }
          >;
      inputs: {};
      params: {
        loader: () => Promise<JSX.Element>;
        defaultPath: string;
        defaultTitle: string;
        routeRef?: RouteRef<AnyRouteRefParams> | undefined;
        filter?: string | ((entity: Entity) => boolean) | undefined;
      };
    }>;
    'entity-card:azure-devops/readme': ExtensionDefinition<{
      kind: 'entity-card';
      name: 'readme';
      config: {
        filter: string | undefined;
      };
      configInput: {
        filter?: string | undefined;
      };
      output:
        | ConfigurableExtensionDataRef<
            React_2.JSX.Element,
            'core.reactElement',
            {}
          >
        | ConfigurableExtensionDataRef<
            (entity: Entity) => boolean,
            'catalog.entity-filter-function',
            {
              optional: true;
            }
          >
        | ConfigurableExtensionDataRef<
            string,
            'catalog.entity-filter-expression',
            {
              optional: true;
            }
          >;
      inputs: {};
      params: {
        loader: () => Promise<JSX.Element>;
        filter?: string | ((entity: Entity) => boolean) | undefined;
      };
    }>;
  }
>;
export default _default;

// (No @packageDocumentation comment for this package)
```