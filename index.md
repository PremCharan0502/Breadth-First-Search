## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/PremCharan0502/Breadth-First-Search/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Breadth First Search
Breadth First Search (BFS) algorithm traverses a graph in a breadthward motion and uses a queue to remember to get the next vertex to start a search, when a dead end occurs in any iteration.

Syntax highlighted code block

   vector <int> v[10] ;  //Vector for maintaining adjacency list explained above
        
    int level[10]; //To determine the level of each node
        
    bool vis[10]; //Mark the node if visited 
        
    void bfs(int s) {
        
        queue <int> q;
        
        q.push(s);
        
        level[ s ] = 0 ;  //Setting the level of the source node as 0
        
        vis[ s ] = true;
        
        while(!q.empty())
        
        {  int p = q.front();
        
            q.pop();
        
            for(int i = 0;i < v[ p ].size() ; i++)
                                
            {      if(vis[ v[ p ][ i ] ] == false)
                                
                {      //Setting the level of each node with an increment in the level of parent node
                                
                    level[ v[ p ][ i ] ] = level[ p ]+1;      
                                
                     q.push(v[ p ][ i ]);
                                
                     vis[ v[ p ][ i ] ] = true;    }     }  } }


For more details see [BFS syntax](https://www.hackerearth.com/practice/algorithms/graphs/breadth-first-search/tutorial/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/PremCharan0502/Breadth-First-Search/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
