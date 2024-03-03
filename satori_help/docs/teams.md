
# Teams

By default, you are a member of your own private team, where your repositories and monitors reside by default. Teams allow you to group monitors, repositories, and people together, each with its own settings and access controls.

## Creating a Team

To create a new team, use the command:

```
satori team create <team-name>
```

This command creates a new team where you can add members, repositories, and monitors.

## Managing Team Members

### Adding Members

To add a member to a team:

```
satori team add-member --team <team-name> --email <member-email>
```

### Removing Members

To remove a member from a team:

```
satori team remove-member --team <team-name> --email <member-email>
```

## Managing Repositories and Monitors

### Adding Repositories to a Team

```
satori team add-repo --team <team-name> --repo <repository-name>
```

### Removing Repositories from a Team

```
satori team remove-repo --team <team-name> --repo <repository-name>
```

### Adding Monitors to a Team

```
satori team add-monitor --team <team-name> --monitor <monitor-name>
```

### Removing Monitors from a Team

```
satori team remove-monitor --team <team-name> --monitor <monitor-name>
```

## Setting Up Team Notifications

Satori supports integrating with various services for team notifications, such as Slack and Discord. To set up notifications:

```
satori team notify --team <team-name> --service <service-name> --config <configuration-details>
```

Replace `<service-name>` with the notification service you're using (e.g., `slack`, `discord`) and `<configuration-details>` with the necessary configuration information for the service.

For more detailed instructions on configuring notifications for specific services, refer to the respective sections in the documentation.

![Screenshot of team notifications setup](img/notifications_setup.png)

Remember, managing teams effectively can streamline your CI/CD workflows and enhance collaboration within your organization.