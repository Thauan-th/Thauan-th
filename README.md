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
