```ruby
class Thauan < Developer
  ROLE     = "Full Stack Developer"
  LOCATION = "Minas Gerais, Brazil"

  def stack
    {
      backend:  %w[Ruby-on-Rails Python],
      frontend: %w[Vue React],
      data:     %w[PostgreSQL Redis Sidekiq],
      infra:    %w[AWS Docker Datadog Sentry]
    }
  end

  def currently
    "Healthtech — regulatory integrations, Rails + Vue, feature-flagged rollouts"
  end

  def focus
    ["performance tuning", "scalable architecture", "code review & mentoring"]
  end
end
```

```console
$ git log --author="Thauan André" --oneline --reverse

c0ffee1  2021-09  init: internship — legacy systems, SQL, version control
a17d3f9  2022-08  feat: full stack delivery — Rails, React, end-to-end ownership
5e2b8c4  2024-05  refactor: promoted to Tech Lead — architecture, reviews, mentoring
9d4a6b0  2026-01  feat: healthtech at scale — regulatory integrations, Rails + Vue
```

```console
$ bundle exec rspec

Thauan
  performance
    ✓ cuts API response time from 3.5s to 180ms (N+1 + Redis caching)
    ✓ holds production uptime above 99.5% on AWS
  quality
    ✓ raises test coverage from 15% to 78%
    ✓ reduces production bugs by 60%
  delivery
    ✓ ships behind feature flags, gradually, without incidents
    ✓ meets regulatory deadlines where late is not an option
  leadership
    ✓ leads Rails teams through architecture and code review
    ✓ mentors junior developers

Finished in 4.2 years (files took 0.09s to load)
8 examples, 0 failures
```
