# ANGULAR
The following are questions and answers for angular:

### NullInjectorError: No provider for _HttpClient!
If you are working with Standalone Components and **HttpClient** you will get this error, the only thing to do is to add **provideHttpClient** inside the app.config.ts:

```
import { provideHttpClient } from '@angular/common/http';
providers: [provideHttpClient()]
```
