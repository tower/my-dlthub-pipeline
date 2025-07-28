# :paperclip: My dltHub Pipeline

> Get started with dltHub and Tower by deploying a simple example pipeline.

This is a basic dltHub pipeline that you can run in Tower. This pipeline is [the
example pipeline that dltHub provides](https://dlthub.com/docs/walkthroughs/create-a-pipeline), which loads data from a GitHub
repository into a DuckDB instance (which is thrown away at the end--but hey,
it's a good example!).

## Deploy this example

To deploy it to Tower, after you've logged in using `tower login`, simply run:

```bash
tower deploy
```

> [!TIP]
> Need a login to Tower? Sign up for our [private beta today](https://tower.dev/#beta)!

You need to provide a dltHub secret, as the documentation describes, which is a
Personal Access Token that the pipeline can use to access GitHub. Follow [the
dltHub
documentation](https://dlthub.com/docs/walkthroughs/create-a-pipeline#2-obtain-and-add-api-credentials-from-github)
with regard to how to create it, then give it to Tower using the Tower CLI:

```bash
tower secrets create --name="dlt.sources.api_secret_key" --value="github_pat_abcdefg1234567"
```

## Learn more about Tower

Want to learn a bit more about how you can deploy dltHub, SQL Mesh, DBT Core,
or any Python project to production without even leaving your console? Here are
a few resources for you!

- :phone: [Tower's webiste](https://tower.dev)
- :books: [Tower documentation](https://docs.tower.dev)
- :dancer: [More Tower examples](https://github.com/tower/tower-examples)
- :gift: [Feedback about Tower](https://feedback.tower.dev/)
