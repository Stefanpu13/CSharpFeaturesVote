CSharpFeaturesVote

Voting app workflow:

visit link -> (single input field for username + btn "continue to voting") 
    disallow voting more than once from given phone. How?
    create cookie if user deletes cookie? 
enter username -> proseed to voting page
voting page
    - a list of accordeons for each version ("CSharpVersion" Component)
        - only one accordeon opened at a time
        - each accordeon contains feature for given version
        - each feature: 
            - is a row with "i" button to the right
                - clicking the "i" button goes to featureInfo page where exmaple and explanation are present
            - can be dragged to "Vote" component - a list of max three features
                - once dragged, feature dissappears from Version
    - a Voting component below the features
        - contains 0..3 dragged features
        - feaautes can be reordered
        - features have "remove" btn - that returns them back to the accordeons    
        feature removed from Voting is put in its original place
    - a Vote btn
        - disabled if not all places are filled
        - OPTIONAL: 
            
            - when clicked - final page with the selected features appears, In this page the features can be reordered, or user can go back to voting
            - page contains list of selected features and "Confirm" btn. When confirm is clicked the user is sent to "Than you" page. After that the user can only access the page with the input (to be clarified
            ) 
