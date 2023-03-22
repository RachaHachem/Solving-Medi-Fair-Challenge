-o-|-o-|-o-|-o-|-o-|-o-|-o-|-o-|-o-|-o-|-o-|-o-|-o-|-o-|-o-|-o-|-o-|-o-|-o-|-o-|-o-|-

                      	MEDI FAIR CAUSAL INFERENCE CHALLENGE
								March 2023
   
					MEDI-FAIR team -- medi-fair@chalearn.org
                                  
-o-|-o-|-o-|-o-|-o-|-o-|-o-|-o-|-o-|-o-|-o-|-o-|-o-|-o-|-o-|-o-|-o-|-o-|-o-|-o-|-o-|-

DISCLAIMER: ALL INFORMATION, SOFTWARE, DOCUMENTATION, AND DATA ARE PROVIDED "AS-IS" 
ISABELLE GUYON AND/OR OTHER CONTRIBUTORS DISCLAIM ANY EXPRESSED OR IMPLIED WARRANTIES, 
INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS 
FOR ANY PARTICULAR PURPOSE, AND THE WARRANTY OF NON-INFRIGEMENT OF ANY THIRD PARTY'S 
INTELLECTUAL PROPERTY RIGHTS. IN NO EVENT SHALL ISABELLE GUYON AND/OR OTHER CONTRIBUTORS 
BE LIABLE FOR ANY SPECIAL, INDIRECT OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER
ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF SOFTWARE, DOCUMENTS, 
MATERIALS, PUBLICATIONS, OR INFORMATION MADE AVAILABLE FOR THE CHALLENGE. 

CONTENTS:

train_set/					Training data
    X_train.csv				Training causal pairs
	X_train_info.csv 		Training causal pairs information
	y_train.csv 			Training labels (0 for no causal link, 1 for A->B, -1 for B->A)

valid_set/					Validation data
	X_valid.csv				Validation causal pairs
	X_valid_info.csv 		Validation causal pairs information

test_set.tar.gz.enc
	X_test.csv				Test causal pairs
	X_test_info.csv 		Test causal pairs information


You need to make submissions on the validation set to get a score. Submit a file looking like the y_train.csv file,
i.e. a CSV file with a header and one line per causal pair. The first column is the ID of the causal pair, the second
column is the score (towards -inf for B->A, 0 for no explainable causal link, +inf for A->B).
The file should be named results.csv and submitted to the challenge website in a zip file.

The test set will be used to compute the final ranking of the teams. It is encrypted. The decryption key will be
provided to the teams that have submitted a valid results.csv file on the validation set when the final phase starts.


CREDIT FOR THE CAUSAL PAIRS:
	Isabelle Guyon : https://guyon.chalearn.org/
