# msr

This is a dataset consisting of the music stretching resistance of 894 songs of various genres.
[Music stretching resistance (MSR)](https://arxiv.org/abs/1701.03274) measures the acceptable range of time stretching rate of music piece for people’s psychoacoustic hearing.
The MSR of a single song consists of two values: *the maximum elongating rate* and *the minimum compressing rate*, 
within which range this song can be *safely* stretched using methods like [WSOLA](https://www.computer.org/web/csdl/index/-/csdl/proceedings/icassp/1993/0946/02/00319366-abs.html).

The distribution of songs with respect to each genre is shown below:
<table>
  	<tr>
		<td>Genre</td>
		<td>#Pieces</td>
		<td>Genre</td>
		<td>#Pieces</td>
		<td>Genre</td>
		<td>#Pieces</td>
	</tr>
	<tr>
		<td>Pop</td>
		<td>87</td>
		<td>Rock</td>
		<td>95</td>
		<td>Easy Listening</td>
		<td>83</td>
	</tr>
	<tr>
		<td>Country</td>
		<td>86</td>
		<td>Folk</td>
		<td>80</td>
		<td>Latin</td>
		<td>68</td>
	</tr>
	<tr>
		<td>Hip-hop&Rap</td>
		<td>82</td>
		<td>R&B</td>
		<td>90</td>
		<td>Jazz&Blues</td>
		<td>78</td>
	</tr>
	<tr>
		<td>Classical</td>
		<td>73</td>
		<td>Electronic</td>
		<td>72</td>
		<td></td>
		<td></td>
	</tr>
</table>

The MSR values of each song are listed in the file *msr.txt*. 
Each line shows the MSR of a unique song with the following format:
*song name \t artist name \t genre \t the minimum compressing rate \t the maximum elongating rate*. 
The fields are separated with *\t*.  

If you are going to use this dataset, please cite the following publications:

<pre>
<code>
@ARTICLE{JunChen:spl13,
	AUTHOR = "Jun Chen and Chaokun Wang",
	TITLE = "Automatic Music Stretching Resistance Classification Using Audio Features and Genres",
	JOURNAL = "IEEE Signal Processing Letters",
	VOLUME = {20},
	NUMBER = {12},
	PAGES = {1249--1252},
	YEAR = {2013}	}

@INPROCEEDINGS{JunChen:mmm14, 
	AUTHOR = {Jun Chen and Chaokun Wang}, 
	TITLE = {RESIC: A Tool for Music Stretching Resistance Estimation}, 
	BOOKTITLE = {International Conference on Multimedia Modeling}, 
	PAGES = {386-389}, 
	YEAR = "2014", }

@ARTICLE{JunChen:arxiv17,
	AUTHOR = {Jun Chen and Chaokun Wang},
	TITLE = {Investigating the role of musical genre in human perception of music stretching resistance},
	JOURNAL = {CoRR},
	VOLUME = {abs/1701.03274},
	YEAR = {2017},
	URL = {http://arxiv.org/abs/1701.03274} }
</code>
</pre>

In [IEEE Signal Processing Letters 2013](http://ieeexplore.ieee.org/document/6636057/?arnumber=6636057), we proposed a MSR classification algorithm combining music content features and genres based on this dataset. 
In [Multimedia Modeling 2014](https://link.springer.com/chapter/10.1007/978-3-319-04117-9_42), we proposed a tool to automatically estimate the MSR of a user-uploaded song and alert the user about the safe and dangerous stretching ranges on the sliding bar. 
It also supports music stretching as well as playing. 
In the [arxiv paper](https://arxiv.org/abs/1701.03274), we conducted thorough analysis on the MSR values in this dataset. Some interesting findings were presented and discussed in detail.
