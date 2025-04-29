# ser334-a-page-replacement-algorithms-solved
**TO GET THIS SOLUTION VISIT:** [SER334 A Page Replacement Algorithms Solved](https://www.ankitcodinghub.com/product/ser334-a-page-replacement-algorithms-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;86354&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;5&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (5 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;SER334 A Page Replacement Algorithms Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (5 votes)    </div>
    </div>
Implement a program that simulates maintaining a page table using three different page replacement algorithms.

write a program that simulates the contents of page table as memory requests are made. This

starts with loading a reference string (a sequence of page numbers) which represents the pages being requested by a specific program. Whenever the program requests a page not already in a frame (i.e., not in physical memory), say that a page fault occurs as the system must load the piece of data into a frame. Typically, there are many more pages (virtual memory) than frames (physical memory), meaning not every page can be loaded with physical memory at the same time. At some point, the program will have a page fault but all frames are being used. This requires to select a particular page for eviction to make space for a new page, and the selection is performed according to some page replacement algorithm.

write a program that simulates a page table. The page table is effectively an array of page entries, where each entry includes a frame number and some other metadata. The metadata includes a so-called valid/invalid bit, which indicates if a particular page is loaded into physical memory (i.e., it exists in some frame). Whenever a program tries to access a particular page (see Simulator.c which loads and uses a specific reference string), it informs the page table. The page table’s job is to make sure pages are loaded when needed. Initially all pages have their valid bit set to zero to represent the fact that nothing is loaded. When a page is accessed, it is brought into memory. For limited simulation, bringing something into memory only means setting it’s valid bit to one to represent that it is loaded (we won’t actually do anything). When there are unused frames, the page table will select the rst unused frame to use rather than use a page replacement algorithm. A page replacement algorithm is used to select which of the existing pages should b e evicted from memory (i.e., have it’s valid bit set to zero) when all frames are in use, so that a new page can b e made to use the frame that the evicted page previously occupied. Your program must support three page replacement algorithms: First-in First-Out (FIFO), Least Recently Used (LRU), Most Frequently Used (MFU). Tie breaking for LRU and MFU should always select the lowest page number (e.g., for MFU, if both page 1 and 2 have the same frequency, replace page 1). Header files are provided.

Your job is to implement a page table and these three page replacement algorithms.

Requirements:

<ol>
<li>c: A file containing a set of functions to load a data file. (This is not a class.) •struct test_scenario* load_test_data(char* lename): Loads the data le and returns a struct containing its information.</li>
<li>c: A file containing a set of functions to simulate a page table.</li>
</ol>
<ul>
<li>struct page_table_entry: Stores general information about a page table entry.</li>
</ul>
-Must use exactly one unsigned int variable to store both the dirty bit and the valid/invalid bit. The right most bit will b e the valid/invalid bit. The second bit from the right will b e the dirty bit. For our simulation, the dirty bit should always be 0.

<ul>
<li>struct page_table: Stores general information about a page table object.</li>
<li>struct page_table* page_table_create(int page_count, int frame_count, enum replacement_algorithm algorithm, int verbose): Initializes the page table.</li>
</ul>
Verbose parameter is for your debugging only – during grading we always set it to 0.

<ul>
<li>void page_table_destroy(struct page_table** pt): Shuts down the page table.</li>
<li>void page_table_access_page(struct page_table *pt, int page): Simulates the program accessing a particular page.</li>
</ul>
Supports putting the storing page into rst free frame if available.

Support FIFO page replacement.

Support LRU page replacement.

Support MFU page replacement.

<ul>
<li>void page_table_display(struct page_table* pt): Displays page table replacement algorithm, number of page faults, and the current contents of the page table.</li>
<li>void page_table_display_contents(struct page_table *pt): Displays the current contents of the page table.</li>
</ul>
You may add other helper functions as needed. The output for the sample data file is given below:

2.1 Verbose Output

This should not b e displayed, we only give it as a suggestion for how to do debugging. For the purposes of troubleshooting, we implemented a more complete output for the program when the verbose option is enabled (see below). This output shows the various pieces of data that each page entry contains.

3 Data File

Your program is required to read in a text file which contains a description of a reference string that will be simulated. The rst line gives the number of pages for the system, the second gives the number of frames, and the third line lists the number of page requests (aka entries) in the reference string. After that, reference string entries are listed in sequence from 0 to the number indicated. All numbers are positive integers. A sample data file is attached to this assignment (not the one we will grade with) and an annotated version is shown below. You may assume that a reference string contains at most 512 entries.

Submission

The submission for this assignment has one part: a source code submission.

Source Code: Please name your main class as “DataLoader.c”, and PageTable.c

<ul>
<li></li>
</ul>
<table>
<tbody>
<tr>
<td width="130"></td>
</tr>
<tr>
<td></td>
<td></td>
</tr>
</tbody>
</table>
<ul>
<li>If your program fails to compile out-of-the-box, there will be a mandatory deduction 20% fromthe assignment points.</li>
<li>If you do not follow the file submission standards (e.g., the submission contains project files,lacks a proper header), there will be a mandatory deduction of 10% from the assignment points. • If compiling or running your program differs from stated on the assignment and it is not specified as a requirement, please include a readme file with steps to execute the program. If you do not, there will be a mandatory 10% deduction from the assignment points</li>
</ul>
