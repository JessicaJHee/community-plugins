## API Report File for "@backstage-community/plugin-3scale-backend"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts
import { BackendFeature } from '@backstage/backend-plugin-api';
import type { Config } from '@backstage/config';
import { EntityProvider } from '@backstage/plugin-catalog-node';
import { EntityProviderConnection } from '@backstage/plugin-catalog-node';
import type { LoggerService } from '@backstage/backend-plugin-api';
import type { SchedulerService } from '@backstage/backend-plugin-api';
import type { SchedulerServiceTaskRunner } from '@backstage/backend-plugin-api';

// @public (undocumented)
const catalogModule3ScaleEntityProvider: BackendFeature;
export default catalogModule3ScaleEntityProvider;

// @public (undocumented)
export class ThreeScaleApiEntityProvider implements EntityProvider {
  // (undocumented)
  connect(connection: EntityProviderConnection): Promise<void>;
  // (undocumented)
  static fromConfig(
    deps: {
      config: Config;
      logger: LoggerService;
    },
    options: {
      schedule: SchedulerServiceTaskRunner;
      scheduler: SchedulerService;
    },
  ): ThreeScaleApiEntityProvider[];
  // (undocumented)
  getProviderName(): string;
  // (undocumented)
  run(): Promise<void>;
}

// (No @packageDocumentation comment for this package)
```
