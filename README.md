# MultiFaaS

MultiFaaS is a Multi-Cloud Functions as a Service toolkit, example, and docs project in its initial brainstorming phase.
The only other file in this repo is the MPL [LICENSE](./LICENSE). The initial [roadmap](#roadmap) is highly likely to change.

## Roadmap <a name="roadmap"></a>

- [ ] github org
- [ ] logo inspired by https://images-na.ssl-images-amazon.com/images/I/41Qjmnse-QL.jpg
  - [ ] find better images
    - https://giphy.com/gifs/rYOlRMcFH9BFS
- [ ] port status.mozmar.org to generic example
- [ ] Jenkinsfile with multibranch pipeline ported from bedrock & basket
  - [ ] infra branches
      - [ ] spin up a k8s cluster
        - [ ] kops
        - [ ] tectonic
        - [ ] gke
      - [ ] install & configure ingress & DNS controllers
      - [ ] helm install jenkins
        - [ ] port jenkins deployment from ee-infra-jenkins ansible
          - [ ] blog post
      - [ ] configure a multibranch pipeline that polls this repo once a minute
  - [ ] kubeless branch
    - [ ] helm install kubeless
    - [ ] helm install minio
    - [ ] helm install kubless-minio-events
      - [ ] find or create repo with equivalent to lambda + s3 events
  - [ ] aws branch
    - [ ] script from infra repo to create s3 + cloudformation + lambda
  - [ ] gcp branch
    - [ ] parity with aws branch
  - [ ] azure branch
    - [ ] parity with aws & gcp branches
  - [ ] dns branches 
  - [ ] docs branch
    - [ ] sphinx tooling and multicloud static site deployment
- related work
  - https://github.com/anaibol/awesome-serverless
  - https://github.com/Miserlou/Zappa 
