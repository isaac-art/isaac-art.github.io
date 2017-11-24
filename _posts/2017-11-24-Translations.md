---
layout: post
title: "Writing"
author: "Isaac "
---

The reading for this week was *Executing Practices* by Helen Pritchard, Eric Snodgrass, Magdalena Tyzlik-Carver. Which takes a prompt from Donald Knuth and introduces different ways of exploring the challange. 

>"Make a thorough analysis of everything your computer does during one second of computation. The computer will execute several hundred thousand instructions during that second;
I’d like you to study them all." (Knuth [1989] 1991, 12–13)

>"the instruction cycle does not encompass excecution's impact and embeddedness in the world" 
Thinking of this text in relation to the research of oour group project made me reconsider how code differs from other forms of writing in its excecution, how it goes on to do something, to go beyond itself as text and language. 

The research I am undertaking started with questions around how language has an impact on a programmer, and how creative coding frameworks impose a way of seeing on an artists. I was wondering how programming languages constrain futures, constrain ways of thinking and solutions to problems that make sense to that language. As an artist I find my primary concern with using programming in my work is around the value transferrence and alignment with the people who created the languages, the frameworks, the tools and material I work with.  
>"processes of computation have particular obligations that infringe upon those who practice or are affected by it."

This research has led to a few different threads I am interested in exploring:

* a study of community and cultural values and exchanges within software (e.g. examining who contributes what, from where, and why certain choices are made, to software such as processing, through an analysis of git history)
* a study of what programming languages are used in different situations, why they are useful for those tasks
* a study of the artwork made using structures such as processing/ openFrameworks 


[Rosetta Code](http://rosettacode.org/wiki/Rosetta_Code) could be a good starting point to see which problems have been solved in multiple languages. 


[code-poetry](http://code-poetry.com/) and [Source Code Poetry Competition
](http://sourcecodepoetry.com/) give examples of people trying to break out of languages. 

------------------

For our artifact project we decided to begin an exploration of the constraints of the words used in programming languages by attempting to write short storys or poems using only the reserved words of languages, in a kind of pseudo-code prose.(see end of page) We have been debating the importance of having compilable code, if it is un-excecutable is it still using the same languague constraints? What is the importance of formatting? Tabs and spaces offer pauses in something not to be read. 

We have been talking about moving into performative versions of these texts, reading something normally silent. Could we take Knuths prompt and act the source code of the opening scenes of startup? 

[loveLetter.vbs reading (2001)](https://transmediale.de/content/lovelettervbs-reading)

-------------
	// a science class
	for char in  class
		try break true using concept explicit
		register union or volatile case
			if catch or break default
				goto friend
				try double 
				if catch or break default
					goto private or public 
						register new concept
			else
				delete and continue
		else
			delete and continue
			
-------------
			
	///
	public friend and private void
	double false operator
	volatile default
	while protected 
		delete public union and throw explicit namespace
		goto register and unsigned inline char 

-------------

	///
	while register namespace protected public
		goto private class


-------------


	void ofApp::setup(){
    
    theSky = ofColor::lightSkyBlue;
    	ofBackground(theSky);
    	family.push_back("Dad");
    	family.push_back("Mum");
    	family.push_back("Sister");
    	family.push_back("Sister");
    	family.push_back("Sister");
    
    	me = 50;
    	nextToMe = me + 10;

    	soTall = 200;
    	notMoving = true;
    	amountItHasTurned = 0;
    	whenWeArrived = ofGetSeconds();
    	secondsWeHaveBeenThere = 0;
	}


	void ofApp::update(){
    	secondsWeHaveBeenThere = ofGetSeconds()-whenWeArrived;
    	if(secondsWeHaveBeenThere > 5){
        	notMoving = false;
        	amountItHasTurned++;
        	nextToMe -= 5;
    	}
	}

	void ofApp::draw(){
    	aSpringGreen = ofColor::springGreen;
    	weWereStandingInTheField(aSpringGreen);
    
    	if(notMoving){
        	theTurbine(soTall, notMoving, amountItHasTurned);
    	}else{
        	theTurbine(soTall, notMoving, amountItHasTurned);
    	}
    	for(int i =0; i< family.size(); i++){
        	int tall = family.size()-i * 10;
        	ofSetColor(255);
       	 ofDrawCircle(nextToMe+(i*40), ofGetHeight()/2, tall);
    	}
	}

	void ofApp::weWereStandingInTheField(ofColor fieldColor){
    	ofSetColor(fieldColor);
    	ofDrawRectangle(0,ofGetHeight()/2,ofGetWidth(),ofGetHeight()/2);
	}


	void ofApp::theTurbine(int height, bool notTurning, float turn){
    
    	ofPushMatrix();
    	ofPushStyle();
    	ofSetColor(255);
    	ofTranslate(600, (ofGetHeight()/2)-height);
    	ofPushMatrix();
    	if(!notTurning){
    	    ofRotate(turn);
    	}
    	ofDrawLine(0, 0, 0, -20);
    	ofDrawLine(0, 0, 20, 20);
    	ofDrawLine(0, 0, -20, 20);
    	ofPopMatrix();
    	ofDrawTriangle(0, 0, -10, height, 10, height);
    	ofPopStyle();
    	ofPopMatrix();
	}
