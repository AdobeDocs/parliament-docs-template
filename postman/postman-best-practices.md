# How to effectively use Postman collections

The quicker you can get users started, the better. One way to jumpstart the configuration of an API is by using Run in Postman buttons. This can reduce more lengthy and tedious explanations about parameters and other configurations for an API.

To see how these Run in Postman buttons work, click this button:

<div class="postman-run-button" style="margin-top:15px; margin-bottom: 15px"
data-postman-action="collection/fork"
data-postman-var-1="3578416-16cf5af1-26e2-4c89-bb99-c6be4e510dcb"
data-postman-collection-url="entityId=3578416-16cf5af1-26e2-4c89-bb99-c6be4e510dcb&entityType=collection"></div>
<script type="text/javascript">
  (function (p,o,s,t,m,a,n) {
    !p[s] && (p[s] = function () { (p[t] || (p[t] = [])).push(arguments); });
    !o.getElementById(s+t) && o.getElementsByTagName("head")[0].appendChild((
      (n = o.createElement("script")),
      (n.id = s+t), (n.async = 1), (n.src = m), n
    ));
  }(window, document, "_pm", "PostmanRunObject", "https://run.pstmn.io/button.js"));
</script>

You can see the many [demos of Run in Postman here](https://www.getpostman.com/integrations/run-button). Many of these demos are listed in [Postman's API Network](https://www.getpostman.com/api-network/).

For details on how to share your Postman collections like this, see [Creating Run in Postman buttons](https://learning.postman.com/docs/publishing-your-api/run-in-postman/creating-run-button/) in the Postman documentation. To try out Run in Postman, you can either [import an OpenAPI spec into Postman](https://www.getpostman.com/docs/postman/collections/data_formats#importing-postman-data) or enter your API information manually.

What's especially good about Postman is that it allows users to customize the API key and parameters and save those values. You can also safely share an API key. Although Postman doesn't provide same direct, in-documentation experience, in many ways the Postman client is more useful because it lets users configure and save the calls they make. They can easily save many different variations of the same endpoint, with different configurations. Postman is what internal developers often use to save and store API calls as they test and explore the functionality.