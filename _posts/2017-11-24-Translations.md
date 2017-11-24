---
layout: post
title: "Writing"
author: "Isaac "
---

For our artifact project we decided to try writing using only the reserved words of languages.

For example, in c++:

`for char in  class
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

public friend and private void
double false operator
volatile default
while protected 
	delete public union and throw explicit namespace
	goto register and unsigned inline char 


while register namespace protected public
	goto private class
`

`
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
`


