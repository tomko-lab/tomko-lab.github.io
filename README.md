# Martin Tomko's Website
The website is built using Hugo static website generator and to run the website locally you should install Hugo first.

## Hugo installation
To install hugo in Linux you can use the following command:

```bash
sudo apt-get install hugo
```

More information about the installation in other operating systems can be found in this link: [Hugo Installation](https://gohugo.io/getting-started/installing/)

### Testing hugo
Run the following script to see everything is set for Hugo or not:

```bash
hugo version
```

## Running the Website:
After installing hugo, you can run the website locally using the following command:

```bash
hugo server
```

There are several parameters that can be set in the aforementioned command. More information are available in the following link: [Parameters](https://gohugo.io/commands/hugo_server/)


## Modifying the website
To modify the content, use the following instructions.

### Adding new posts (basic)
Posts are by default are shown in the home page and they can be accessed and filtered by tags and categories.
To add a new post use the following command:

```bash
hugo new posts/[NAME_OF_YOUR_POST]
```

Then, a new markdown file will be created in *'content/posts'* folder. Add the tags and contents to this file and that's it!

In order to add figures or social media content to your post, use the following instructions.

### Adding new posts (figures)
First, add the image(s) in *'static/images'* folder. Then use the following script in your code to add the image to the content of your post:

```markdown
![DESCRIPTION_OF_THE_IMAGE](/images/NAME_OF_THE_IMAGE)
```

### Adding new posts (sharing content from social media)
To share social media content in your post you can use the Hugo Shortcodes that available for Twitter, Facebook, Instagram and Youtube. You can find full details in the following link: [](). In the following, an example of using the Twitter shortcode is provided (NOTE: the *1391890227476766727* is the tweet id).

```markdown
{{< tweet 1391890227476766727 >}}
```

### Adding new team member
To add new person to the link, first you should edit the people JSON file in *data/people.json* and add information about the new person including name, email and title. There is a specific field that you should provide as well, **page**. Page attribute should be name of the profile page which will be generated in the next step.

Add a new page as the profile page for the member using the following command:

```bash
hugo new people/[PAGE_NAME]
```
