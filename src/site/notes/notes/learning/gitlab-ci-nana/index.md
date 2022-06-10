---
{"dg-publish":true,"permalink":"/notes/learning/gitlab-ci-nana/index/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# GitLab CI/CD - From Zero to Hero

by Nana

<https://techworld-with-nana.teachable.com/courses/enrolled/1769488>

---

## Things to try at work

- [ ] deploy jobs should have the name of the environment (dev/stage/us-prod/ca-prod)
- [ ] tests generating a JUnit report <https://www.npmjs.com/package/jest-junit>
- [ ] integrate the JUnit report with GitLab's UI <https://docs.gitlab.com/ee/ci/yaml/artifacts_reports.html#artifactsreportsjunit>
- [ ] use the environment keyword in the deploy job <https://docs.gitlab.com/ee/ci/yaml/#environment>
- [ ] use the `artifacts:report:dotenv` to pass environment variables to the next stages/jobs <
- [ ] use cache based on changes in `package.json` (and/or lock files)
    - depends on removing tests from cloudbuild
    - <https://docs.gitlab.com/ee/ci/caching/>
    - advanced `config.toml` configuration: <https://docs.gitlab.com/runner/configuration/advanced-configuration.html>
- use GitLab's SAST (but with `allow_failure`): <https://docs.gitlab.com/ee/user/application_security/sast/>
    - I've noticed in the `gl-sast-report.json` that some vulnerabilities were found but the job finished successfully.


---


Nothing really new for me in sections 1, 2 and 3.

- [[notes/learning/gitlab-ci-nana/4 - GitLab Architecture|4 - GitLab Architecture]]
- [[notes/learning/gitlab-ci-nana/5 - CI-CD pipeline for Node.js Application|5 - CI-CD pipeline for Node.js Application]]
- [[notes/learning/gitlab-ci-nana/6 - Optimize CI-CD Pipeline & Configure Multi-Stage Pipeline|6 - Optimize CI-CD Pipeline & Configure Multi-Stage Pipeline]]
- [[notes/learning/gitlab-ci-nana/7 - CI-CD MicroService Application (Mono and Polyrepo)|7 - CI-CD MicroService Application (Mono and Polyrepo)]]
- [[notes/learning/gitlab-ci-nana/8 - Deploy Microservices to Kubernetes cluster|8 - Deploy Microservices to Kubernetes cluster]]

