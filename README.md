# 微前端示例项目

整个项目为一个多包项目(Monorepo)，项目使用 lerna-lite 结合 pnpm 的 workspace 进行多包管理

- 微前端是一种将大型前端应用程序拆分为小的、松耦合的部分的方法，以便不同的部分可以独立地开发、测试和部署。

- Monorepo 是一种开发方法，它使用相同的代码库来管理多个项目。在微前端中，Monorepo 是一种将微服务应用程序代码打包到一个代码库中的方法，而不是将每个微服务应用程序作为单独的代码库处理。这使得跨多个微服务应用程序共享代码和库变得更加容易，并且可以减少重复代码，从而提高开发效率和代码质量。同时，Monorepo 还提供了更好的版本控制和协作，使得更容易协调代码库中的变更。使用 Monorepo 还可以使团队更容易协作和跟踪整个应用程序的开发进度和版本历史记录。

- 使用 Monorepo 的微前端项目可以采用以下步骤：

  1. 创建一个单独的代码库，用于存储所有微前端应用程序的代码。

  2. 在代码库中创建一个根项目，该项目将承担所有微前端应用程序之间的通信和路由管理职责。这个根项目可以是一个单独的微前端应用程序，也可以是专门用于管理微前端的工具库。

  3. 在代码库中创建多个子项目，每个子项目对应一个微前端应用程序。每个子项目都应该只处理自己的业务逻辑，且应该独立测试、构建和部署。子项目可以共享代码和库。

  4. 将子项目集成到根项目中，这样根项目就可以路由请求给不同的子项目。

  5. 使用适当的工具和框架，如 Webpack，Module Federation 和 Single-SPA，来协调不同的微前端应用程序之间的通信和部署。这些工具和框架可以帮助处理工程化和运行时的代码解耦。

  6. 确保在开发、测试和部署微前端应用程序时，子项目的代码和配置文件可以独立管理，而不会影响其他子项目。通过 Monorepo 管理不同微前端应用程序的代码，可以更好地管理和协调这些应用程序之间的关系。

使用 Monorepo 的微前端项目可以带来更高的开发效率、更好的代码质量，以及更好的协作支持。

# TODO

- 在根目录使用统一的环境变量
