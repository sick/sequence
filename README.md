sequence
========

Sequence module from awesome cgkit library
http://cgkit.sourceforge.net/doc2/sequence.html

Quick example
	import sequence
	sequences = sequence.glob('pattern or path to directory or partial name')

    for seq in sequences:
        ff = str(seq[0]) #Firts frame
        lf = str(seq[-1]) #Last frame
        name, range = seq.sequenceName() #Sequence name and Range object
        path, filename = os.path.split(name) 
        root, ext = os.path.splitext(filename) #get extension and name
        count = len(range) # Frame count - sequence length 
        frames = list(range)
        fframe = str(frames[0]) #Firts frame digit, 1
        lframe = str(frames[-1]) #Last frame digit, 89

And better examples is here http://cgkit.sourceforge.net/doc2/filesequencetools.html