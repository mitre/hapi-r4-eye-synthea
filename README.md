# HAPI with Synthetic Eye Data

Builds on <https://github.com/smart-on-fhir/hapi> to create a Docker container that contains synthetic data augmented with eye data elements.

To run, first clone this repository and open a command line window to run the following:

```shell
docker build . --tag "hapi-r4-eye-synthea"
docker run -it -p 8080:8080 hapi-r4-eye-synthea
```

While this container is running, FHIR endpoints like `http://localhost:8080/hapi-fhir-jpaserver/fhir/Patient` should yield responses with the pre-populated synthetic data.

----

## License

Copyright 2023 The MITRE Corporation

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

----

MITRE: Approved for Public Release / Case #24-0169
