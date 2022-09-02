nodemon 试试监听js文件修改，自动刷新

fastify[https://www.fastify.io/] 快速并且低开销的 web 框架，专为 Node.js 平台量身打造。

```js
const fastify = require("fastify")({ logger: true });

fastify.get("/", async function name(req, res) {
  return { hello: "world" };
});

const start = async () => {
  try {
    await fastify.listen({ port: 3000 });
  } catch (error) {
    fastify.log.error(err);
    process.exit(1);
  }
};

start();

```


sharp[https://sharp.pixelplumbing.com/]
图像处理

