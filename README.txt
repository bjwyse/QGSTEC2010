Question Generation Shared Task & Evaluation Challenge (QGSTEC) 2010 Resources

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.

Summary
=======
The first Question Generation Shared Task & Evaluation Challenge took
place in 2010. The purpose of the challenge was to advance research
in the Natural Language Processing and Generation sub-field of 
Question Generation (QG). The files in this archive are the resources
used in that challenge including final submissions and ratings.

Task B Contents
===============

Task B was a task to generate questions from one single sentence.
The task consisted of an initial development data set release to
allow participants to set up their systems and to get an idea as to
how the challenge would be carried out. This initial data set is
available in the DevData folder.

The XML format in the TestData folder is the finalised format which
includes tags for raters and their ratings. Also included in this
folder is the XSLT file used to translate the ratings into a table.

The table was exported to Excel to calculate various results. There
are three spreadsheets which varying degrees of information presented.

The XML schema consisted of a root 'dataset' element with a child element
called 'instance' for each test instance. The 'text' element contained
the input to the QG system and the 'targetQuestionType' element specified
the question type to be generated.

Participant's submissions are in the 'submission' element with the corresponding
ratings according to the various criteria as attributes.

Example:
----------------------------------------------------------------------------------
<dataset>
<instance id="1">
	<id>OpenLearn</id>
	<source>A103_3</source>
	<text>The view that prevailed was that there should be a fitting public memorial to the 49,076 gunners who died.</text>
	<targetQuestionType>how many</targetQuestionType>
	<submission id="a">
		<question type="how many">To the how many gunners who died was the idea that prevailed there should be a public fitting memorial?
		<rating rater="ss" relevance="1" questionType="1" correctness="4" ambiguity="1" variety="2" />
        <rating rater="ha" relevance="1" questionType="1" correctness="1" ambiguity="1" variety="2" />
		</question>
		<question type="how many">The how many gunners who died was the idea that prevailed there should be a public memorial fitting to?
		<rating rater="ss" relevance="4" questionType="1" correctness="4" ambiguity="1" variety="2" />
        <rating rater="ha" relevance="1" questionType="1" correctness="2" ambiguity="1" variety="2" /> 
		</question>
	</submission>
</instance>
----------------------------------------------------------------------------------

For further information on QGSTEC2010 and these resources, contact: Brendan Wyse <bjwyse@gmail.com>
