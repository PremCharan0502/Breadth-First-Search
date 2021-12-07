## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/PremCharan0502/Breadth-First-Search/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Breadth First Search
Breadth First Search (BFS) algorithm traverses a graph in a breadthward motion and uses a queue to remember to get the next vertex to start a search, when a dead end occurs in any iteration.

Syntax highlighted code block

#include <iostream>
using namespace std;

int main()
{//for first time
	int hour1,minute1,second1;
	//for second time
	int hour2,minute2,second2;
	//for the total(sum) time
	int hour,minute,second;
	//taking the input from user
	cout<<"***Enter first time***"<<endl;
	cout<<"Hours: "; cin>>hour1;
	cout<<"Minutes: "; cin>>minute1;
	cout<<"Seconds: "; cin>>second1;
	//taking the input from user
	cout<<"***Enter second time***"<<endl;
	cout<<"Hours: "; cin>>hour2;
	cout<<"Minutes: "; cin>>minute2;
	cout<<"Seconds: "; cin>>second2;
	//adding the entered times
	second=second1+second2;
	minute=minute1+minute2+(second/60);
	hour=hour1+hour2+(minute/60);
	minute=minute%60;
	second=second%60;
	//displaying total time
	cout<<"Total Time is: "<<hour<<" hours "<<minute<<" minutes "<<second<< " seconds";
return 0;}

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/PremCharan0502/Breadth-First-Search/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
