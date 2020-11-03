*** AMG1608 Dataset ***

This dataset contains 1608 songs with valence-arousal (VA) labels annotated by 665 users recruited from the Internet.
The data are saved as MATLAB MAT-file, which is named as "AMG1608.mat."
AMG1608.mat has three variables, they are:
- feat_cell
- song_info
- song_label
The description of each variable is given in what follows.

feat_cell:
This is a 1608-by-1 cell matrix that contains the frame-level acoustic feature vectors of the songs.
Each cell is the collection of frame-level feature vectors of a song. 
The collection of feature vectors is a D-by-F by matrix, where D denotes the feature dimension and F denotes the frame numbers.
Specifically, D=72 and F=1199 in this dataset.
Please refer to "feature_index.txt" for the descriptions and indices of the feature sets used.

song_info:
This is a 1608-by-2 cell matrix.
Each element in the first column is the artist name of each song and each element in the second column is the song title of the song.

song_label:
This is a 1608-by-665-by-2 cubical matrix that contains the VA annotations of the songs.
The three dimensions of this matrix corresponds to the song index, user index, and emotion index, respectively.
In particular, the affective valence corresponds to the emotion index=1 and affective arousal corresponds to the emotion index=2.
