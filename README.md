🧱 Create Article Collection Type
Go to Content-Type Builder

Create a new Collection Type named: karthik-Article

Add the following fields:

title (tasknumber)

content (details)
Save the schema and allow Strapi to restart.

done or not (boolean)
🧑‍🔧 Configure Public Permissions
Go to: Settings > Roles > Public

Under Article, enable:

find

findOne

Save the permissions

📝 Add and Publish Content
Go to Content Manager > Articles

Click Create new entry

Fill in the fields, and click Publish



GET http://localhost:1337/api/articles

