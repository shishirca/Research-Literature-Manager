# Research Literature Manager

This is a project that makes it simple to manage the research papers you have read!

## How to use

### Setting up the Repository

1. Click on the `Use this template` button to make a copy of this repository to your own Github account.
   ![Use this template button](assets/1.jpg)
2. Open the file `papersToAdd.txt` in the GitHub editor, and paste the links of the papers you want to add in the file (one link in each line) and commit the chanegs.

After this, automated actions with fire which will use Semantic Scholar to fetch details about those papers, and then subsequently fetch some candidate papers which might be relevant to your project.

After the actions are complete, you can explore the `data` folder, which will have the following files updated:

- `records.json`: Contains all the information about the papers that you added.
- `currentPapers.csv`: Contains formatted information about the papers currently in the database.
- `candidatePapers.csv`: Contains formatted information about possible candidate papers for your database.

### Setting up the website

The projects ships with a simple website that you can use to easily view and visualise the papers you have listed. We will use `Netlify` to deploy the website once, which would then be updated automatically on every subsequent commit by Netlify's servers!

1. Go to [Netlify](https://www.netlify.com/) and Sign Up/Login with your Github Account.
   ![Step 1](assets/website/1.jpg)
2. Netlify will ask you to allow access to your Github account (if you are using Netlify for the first time). Go ahead and grant it, it's 100% safe!
   ![Step 2](assets/website/2.jpg)
3. On your Netlify dashboard, click on `Import from Git` under the `Sites` section and choose `Github` as your provider.
   ![Step 3-A](assets/website/3.jpg)
   ![Step 3-B](assets/website/4.jpg)
4. In the `Pick your repository` step, choose the repository that you created from the template in the previous step.
   ![Step 4](assets/website/5.jpg)
5. In the next `Basic Build Settings` page, ensure that your settings are configured to these (these should be automatically be filled for you, but it never hurts to double check)!
   ![Step 5](assets/website/6.jpg)
6. Wait for Netlify to deploy your site! After the deployment is complete, your site would get a public URL that you can bookmark and use to view your papers any time!
   ![Step 6](assets/website/7.jpg)

##### Optional Step

You can go to your `Site Settings`, and then under the `Domain Management` Section, you can click on the `Domains` option to edit your randomly generated site name to something a little more you!
![Optional Step](assets/website/8.jpg)

### Note

If some papers could not be found using the links provided, those papers would be left in the `papersToAdd.txt` itself. You can try replacing them with some other link to add them to the database using the scripts.

The scripts and Semantic Scholar API works best with `arxiv` and `semanticScholar` links, so try to use them as much as possible.

### Sample Input

Here is a sample list of papers related to `Numbers in Text` that you can directly put in the `papersToAdd.txt` to quickly checkout the actions:-

```
https://arxiv.org/abs/1803.02155
https://arxiv.org/abs/1808.09637
https://arxiv.org/abs/1809.05356
https://arxiv.org/abs/1909.03065
https://arxiv.org/abs/1910.06611
https://arxiv.org/abs/1912.13283
https://arxiv.org/abs/2003.07629
https://arxiv.org/abs/2004.02363
https://arxiv.org/abs/2004.07085
https://arxiv.org/abs/2004.08500
https://arxiv.org/abs/2004.12193
https://arxiv.org/abs/2005.00242
https://arxiv.org/abs/2005.00683
https://arxiv.org/abs/2005.08516
https://arxiv.org/abs/2005.08517
https://arxiv.org/abs/2006.01681
https://arxiv.org/abs/2006.03274
https://arxiv.org/abs/2006.06609
https://arxiv.org/abs/2006.15595
https://arxiv.org/abs/2008.11990
https://arxiv.org/abs/2010.06666
https://arxiv.org/abs/2010.06973
https://arxiv.org/abs/2102.13019
https://arxiv.org/abs/2103.03874
https://arxiv.org/abs/2103.07191
```
